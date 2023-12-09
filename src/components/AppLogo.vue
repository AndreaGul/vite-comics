<script>
export default {
    name : 'Logo',
    data(){
        return{
            logo: '/img/dc-logo.png',
            
        }
    }
}

</script>

<template>
    <div>
        <img v-bind:src="logo" alt="Logo">
    </div>
</template>

<style>
</style>