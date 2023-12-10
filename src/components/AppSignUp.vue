<script>
export default {
    name : 'SignUp',
    data(){
        return{
            signUp: {
                name: 'Sign-Up Now!',
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

<style scpoed lang="scss">
@use '../styles/partials/variables' as *;
    button{
        border: $primary-celeste solid 3px;
        padding: 16px 14px ;
        cursor: pointer;

        a{
            color: white;
            font-size: 18px;
           
            text-transform: uppercase;
        }
    }
</style>