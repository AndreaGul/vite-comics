<script>
export default {
    name : 'Social',
    data(){
        return {
            category: 'Follow us',
            Links: [
            {
                name: 'Facebook',
                img: '/img/footer-facebook.png',
                link: '#',
                target: '_self',
                
            },
            {
                name: 'Twitter',
                img: '/img/footer-twitter.png',
                link: '#',
                target: '_self',
                
            },
            {   
                name: 'Youtube',
                img: '/img/footer-youtube.png',
                link: '#',
                target: '_self',
                
            },
            {   
                name: 'Pinterest',
                img: '/img/footer-pinterest.png',
                link: '#',
                target: '_self',
                
            },
            {
                name: 'periscope',
                img: '/img/footer-periscope.png',
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
        <li v-for="link in Links">
            <a :href="link.link" :target="link.target"><img :src="link.img" alt=""></a>
            
        </li>
    </ul>
</template>

<style scoped lang="scss">

ul {
    display: flex;
    align-items: center;
    
    
 }
</style>