<!-- JS -->
<script>
// Import
import AppHeaderVue from "./components/AppHeader.vue";
import AppMainVue from "./components/AppMain.vue";
import AppFooterVue from "./components/AppFooter.vue";
export default {
  components: {
    AppHeaderVue,
    AppMainVue,
    AppFooterVue,
  },
  data() {
    return {};
  },
};
</script>

<!-- HTML -->
<template>
  <!-- HEADER -->
  <AppHeaderVue />
  <!-- MAIN -->
  <AppMainVue />
  <!-- FOOTER -->
  <AppFooterVue />
</template>

<!-- SASS -->
<style lang="scss">
@use "../styles/general.scss" as *;
</style>
