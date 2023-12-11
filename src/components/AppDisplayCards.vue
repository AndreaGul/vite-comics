<script>
export default {
    props: {
        image: String,
        title: String,  
    }
};
</script>

<template>
    <div class="img-container">
        <img :src="image" :alt="title">
    </div>
</template>

<style lang="scss" scoped>
</style>