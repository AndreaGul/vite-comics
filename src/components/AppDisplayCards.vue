<script>


export default {
  name: 'DisplayCards',

  props: ['image','title'],
};

</script>

<template>

  
     <li class="card-container"> 
        <div class="img-container">
          
            <img :src="image" :alt="title">

            <h3>{{ title }}</h3>
        </div>
      </li>
</template>

<style lang="scss" scoped>
  p{ color: white;}
</style>