<script>
import AppSignUp from './AppSignUp.vue';
import AppSocial from './AppSocial.vue';
export default {
    name : 'BottomBar',

    components: {
        AppSignUp,
        AppSocial,
    }
}

</script>

<template>
    <footer class="container" >
        <AppSignUp/>
    <AppSocial/>
</footer>
    
</template>

<style scoped lang="scss">
@use '../styles/partials/variables' as *;

 footer {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 34px 0;
    background-color: $primary-dark-grey;
 }
</style>