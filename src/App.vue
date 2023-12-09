<script>
  import AppHeader from './components/AppHeader.vue';
  import AppMain from  './components/AppMain.vue';
  import AppFooter from './components/AppFooter.vue';

  export default {
    name: 'Body',
    components: {
      AppHeader,
      AppMain,
      AppFooter,
    }
  }
</script>

<template>
  <div class="container"><AppHeader />
  <AppMain/>
  <AppFooter/></div>
  
</template>

<style lang="scss">
@use './styles/partials/variables' as *;
@use './styles/general.scss' as *;

.container {
  width: 80%;
  height: 100%;
  margin: 0 auto;
}
</style>
