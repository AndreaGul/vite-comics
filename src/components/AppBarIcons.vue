<script>
export default {
    name : 'SignUp',
    data(){
        return{
            icons: [
                {
                    name: 'Digital comics',
                    img: '/img/buy-comics-digital-comics.png',
                    link: '#',
                    target: '_self',
                },
                {
                    name: 'DC Merchandise',
                    img: '/img/buy-comics-merchandise.png',
                    link: '#',
                    target: '_self',
                },
                {
                    name: 'Subscription',
                    img: '/img/buy-comics-subscriptions.png',
                    link: '#',
                    target: '_self',
                },
                {
                    name: 'Comic shop locator',
                    img: '/img/buy-comics-shop-locator.png',
                    link: '#',
                    target: '_self',
                },
                {
                    name: 'DC power visa',
                    img: '/img/buy-dc-power-visa.svg',
                    link: '#',
                    target: '_self',
                },
            ]
        }
    },
}

</script>

<template>
    <footer>
        <div class="container">   
            <ul>
        <li v-for="text in icons">
            <a :href="text.link" :target="text.target">
                <div class="img-container">
                    <img :src="text.img" :alt="text.name">
                </div>
                <p>{{ text.name  }}</p>
            </a>
            
        </li>
    </ul>
        </div>
    </footer>
    
</template>

<style scoped lang="scss">
@use '../styles/partials/variables' as *;
    

footer{
    background-color: $primary-celeste;
}
    ul {
        display: flex;
        justify-content: space-around;
        padding: 50px;
        
        li {
            

            a {
                display: flex;
                align-items: center;
                
                
                
                
                .img-container{
                    height: 55px;
                    
                    img {
                    display: block;
                    
                    height: 100%;
                    }
                }
                

                p {
                    color: #ffffff;
                    text-transform: uppercase;
                    margin: 0 16px;
                }
            }
           
            
            
        }
    }
   
</style>