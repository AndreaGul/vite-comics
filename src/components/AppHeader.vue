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
@use '../styles/partials/variables' as *;
header {
    display: flex;
    justify-content: space-between;
    align-items: center;
}
</style>