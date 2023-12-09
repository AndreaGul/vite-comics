<script>
import AppLogo from './AppLogo.vue';
import AppNavbar from './AppNavbar.vue';
export default {
    name : 'Headers',

    components:{
        AppLogo,
        AppNavbar,
    }
}

</script>

<template>
    <header><AppLogo/>
        <AppNavbar/></header>
</template>

<style>
</style>