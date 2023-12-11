<script>
import AppMainCard from './AppMainCard.vue';

export default {
    name : 'Main',
    components:  {
        AppMainCard,
    }
}

</script>

<template>
    <header >
        <div class="container"> 
            <AppMainCard/>
        </div>
    </header>
</template>

<style scoped lang="scss">
@use '../assets/scss/partials/variables' as *;


header {
    background-color: $primary-light-black;

   
}


</style>