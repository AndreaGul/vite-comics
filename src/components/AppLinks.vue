<script>
export default {
    name : 'Links',
    data(){
        return{
            category: 'Dc Comics',
            navbarLinks: [
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
                
        }
    }
}

</script>

<template>
    <ul>
        <li><h2>{{ category }}</h2></li>
        <li v-for="link in navbarLinks">
            <a :href="link.link" :target="link.target">{{ link.name }}</a>
            
        </li>
        
    </ul>
    <ul>
        <li><h2>{{ category }}</h2></li>
        <li v-for="link in navbarLinks">
            <a :href="link.link" :target="link.target">{{ link.name }}</a>
            
        </li>
        
    </ul>
    <ul>
        <li><h2>{{ category }}</h2></li>
        <li v-for="link in navbarLinks">
            <a :href="link.link" :target="link.target">{{ link.name }}</a>
            
        </li>
        
    </ul>
</template>


<style>
</style>