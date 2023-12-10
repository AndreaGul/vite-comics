<script>
export default {
    name : 'Main',
    data (){
        return{
            text: '--> Contenti goes here <--',
        }
    }
}

</script>

<template>
    <header >
        <div class="container"> 
            <p>{{text}}</p>
        </div>
    </header>
</template>

<style scoped lang="scss">
@use '../styles/partials/variables' as *;


header {
    background-color: $primary-light-black;

    .container {
    padding: 56px 0;
    p{
        color: #ffffff;
        font-size: 20px;
    }
    }
}


</style>