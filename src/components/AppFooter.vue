<script>
import AppLinks from './AppLinks.vue';
import AppBottomBar from './AppBottomBar.vue';
import AppBarIcons from './AppBarIcons.vue';

export default {
    name : 'Footer',
    components: {
        AppLinks,
        AppBottomBar,
        AppBarIcons,
    }
}

</script>

<template>
   <footer>
    <AppBarIcons/>
    <AppLinks />
    <AppBottomBar/>
    </footer>
</template>

<style scoped lang="scss">
 

</style>