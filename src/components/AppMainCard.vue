

<script>
import AppDisplayCards from './AppDisplayCards.vue';
export default {
    name : 'Card',
    components: {
        AppDisplayCards,
    },
    data(){
        return {
           
            cards: [
                {
                        "thumb": "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
                        "series": "Action Comics",
                },
                {
                    "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
                    "series": "American Vampire 1976",
                },
                {
                    "thumb": "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
                    "series": "Aquaman",
                },
                {
                    "thumb": "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
                    "series": "Batgirl",
                },
                {
                    "thumb": "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
                    "series": "Batman",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
                    "series": "Batman Beyond",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
                    "series": "Batman/Superman",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
                    "series": "Batman/Superman Annual",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
                    "series": "Batman: The Joker War Zone",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
                    "series": "Batman: Three Jokers",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
                    "series": "Catwoman",
                },
            ]
        }
    },

    
   
}

</script>

<template>
    <div class="cards-container">
        <ul  class="cards" >
            <AppDisplayCards v-for="card in cards" 
                :image="card.thumb" 
                :title="card.series"
            />
            <!-- <li v-for="card in cards" class="card-container"> 
                <div class="img-container">
                
                    <img :src="card.thumb" :alt="card.series">
                    <h3>{{ card.series }}</h3>
                </div>
            </li> -->
          <!-- <AppDisplayCards  :image="card.thumb" :title="card.series"/> -->
        </ul>
    </div>
</template>

<style scoped lang="scss">
    .cards-container{
        padding: 55px 0;
        .cards {
            display: flex;
            flex-wrap: wrap;
            gap: 30px;

                :deep(.card-container) {
                    width: calc((100% - (30px *5 )) / 6);
                    
                    
                    .img-container {
                    aspect-ratio: 1/1;
                    
                        img{
                            height: 100%;
                            width: 100%;
                            object-fit: cover;
                            
                        }
                    
                    }

                    h3 {
                        text-align: center;
                        color: white;
                        margin: 20px 0;
                    }

                    
                    }
        }
    }
        
    

</style>