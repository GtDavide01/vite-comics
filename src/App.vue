<!-- JS -->
<script>
// Import
import AppHeaderVue from './components/AppHeader.vue';
import AppMainVue from './components/AppMain.vue';
export default{
    components: {
      AppHeaderVue,
      AppMainVue,
    }
  }
</script>



<!-- HTML -->
<template>
    <!-- HEADER -->
    <AppHeaderVue/>
    <!-- MAIN -->
    <AppMainVue />
    <!-- FOOTER -->
</template>



<!-- SASS -->
<style lang="scss">
@use "../styles/general.scss" as *;
</style>