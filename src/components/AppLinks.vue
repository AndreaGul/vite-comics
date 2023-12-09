<script>
export default {
    name : 'Links',
    data(){
        return{
            infoLinks: [
                {
                    category: 'DC Comics',
                    Links: [
                    {
                        name: 'Characters',
                        link: '#',
                        target: '_self',
                        
                    },
                    {
                        name: 'Comics',
                        link: '#',
                        target: '_self',
                        
                    },
                    {
                        name: 'Movies',
                        link: '#',
                        target: '_self',
                        
                    },
                    {
                        name: 'Tv',
                        link: '#',
                        target: '_self',
                        
                    },
                    {
                        name: 'Games',
                        link: '#',
                        target: '_self',
                        
                    },
                    {
                        name: 'Collectibles',
                        link: '#',
                        target: '_self',
                        
                    },
                    {
                        name: 'Videos',
                        link: '#',
                        target: '_self',
                        
                    },
                    {
                        name: 'Fans',
                        link: '#',
                        target: '_self',
                        
                    },
                    {
                        name: 'News',
                        link: '#',
                        target: '_self',
                        
                    },
                    {
                        name: 'Shop',
                        link: '#',
                        target: '_self',
                        
                    },
                    ]
                },
                {
                    category: 'Shop',
                    Links: [
                    {
                        name: 'Shop DC',
                        link: '#',
                        target: '_self',
                        
                    },
                    ]
                }
            ]
           
        }
    }
}

</script>

<template>
    <ul v-for="info in infoLinks">
        <li><h2>{{ info.category }}</h2></li>
        <li v-for="link in info.Links">
            <a :href="link.link" :target="link.target">{{ link.name }}</a>
            
        </li>
        
    </ul>
    
</template>


<style>
</style>