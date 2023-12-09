<script>
export default {
    name : 'Navbar',
    data(){
        return{
           navbarLinks: [
            {
                name: 'Characters',
                link: '#',
                target: '_self',
                active: false,
            },
            {
                name: 'Comics',
                link: '#',
                target: '_self',
                active: true,
            },
            {
                name: 'Movies',
                link: '#',
                target: '_self',
                active: false,
            },
            {
                name: 'Tv',
                link: '#',
                target: '_self',
                active: false,
            },
            {
                name: 'Games',
                link: '#',
                target: '_self',
                active: false,
            },
            {
                name: 'Collectibles',
                link: '#',
                target: '_self',
                active: false,
            },
            {
                name: 'Videos',
                link: '#',
                target: '_self',
                active: false,
            },
            {
                name: 'Fans',
                link: '#',
                target: '_self',
                active: false,
            },
            {
                name: 'News',
                link: '#',
                target: '_self',
                active: false,
            },
            {
                name: 'Shop',
                link: '#',
                target: '_self',
                active: false,
            },
           ]
            
        }
    }
}

</script>

<template>
    <ul>
        <li v-for="link in navbarLinks" :class="{active: link.active}">
            <button><a :href="link.link" :target="link.target">{{ link.name }}</a></button>
            
        </li>
        
    </ul>
</template>

<style>
 .active {
 background-color: red;
 }
</style>