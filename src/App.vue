<template>
  <layout-app>
    <router-view />
  </layout-app>
</template>
<script>
// globel layout Navbar//
import LayoutApp from "./components/Globel/LayoutApp.vue";
export default {
  components: {
    LayoutApp,
  },
};
</script>
<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
