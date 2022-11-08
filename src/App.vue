<!-- JS -->
<script>
// Import
import AppHeaderVue from './components/AppHeader.vue';
export default{
    components: {
      AppHeaderVue,
    }
  }
</script>



<!-- HTML -->
<template>
  <div class="container">
    <!-- HEADER -->
    <AppHeaderVue/>
  </div>
  
</template>



<!-- SASS -->
<style lang="scss">
@use "../styles/general.scss" as *;
</style>