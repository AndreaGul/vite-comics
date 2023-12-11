<script>
import AppLogo from './AppLogo.vue';
import AppNavbar from './AppNavbar.vue';
export default {
    name : 'Headers',

    // data(){
    //     return{
    //     

    //     }
    // }

    components:{
        AppLogo,
        AppNavbar,
    }
}

</script>

<template>
    <header class=" container"><AppLogo/>
        <AppNavbar/></header>
</template>

<style scoped lang="scss">
@use '../assets/scss/partials/variables' as *;

header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px 0;
}
</style>