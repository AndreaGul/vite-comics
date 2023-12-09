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
    <AppSignUp/>
    <AppSocial/>
</template>

<style>
</style>