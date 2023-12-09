<script>
export default {
    name : 'SignUp',
    data(){
        return{
            signUp: {
                name: 'SignUp',
                link: '#',
                target: '_self',
            },
        }
    },
}

</script>

<template>
    <button><a :href="signUp.link" :target="signUp.link">{{ signUp.name }}</a></button>
</template>

<style>
</style>