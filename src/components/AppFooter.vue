<script>
import AppLinks from './AppLinks.vue';
import AppBottomBar from './AppBottomBar.vue';
export default {
    name : 'Footer',
    components: {
        AppLinks,
        AppBottomBar,
    }
}

</script>

<template>
   <footer>
    <AppLinks id="AppLinks"/>
    <AppBottomBar/>
    </footer>
</template>

<style scoped lang="scss">
 

</style>