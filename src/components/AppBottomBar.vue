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
    <footer  >
        <div class="container">
            <AppSignUp/>
            <AppSocial/>
        </div>
      
</footer>
    
</template>

<style scoped lang="scss">
@use '../assets/scss/partials/variables' as *;


 footer {
    
    background-color: $primary-dark-grey;

    .container{
        display: flex;
        align-items: center;
        justify-content: space-between;
        padding: 34px 0;
    }
 }


</style>