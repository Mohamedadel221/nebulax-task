<template>
  <div>
    <v-layout>
      <v-main style="padding-top: 50px">
        <slot></slot>
      </v-main>
      <NavBar />
    </v-layout>
  </div>
</template>

<script>
import NavBar from "./NavBar.vue";
export default {
  components: {
    NavBar,
  },
};
</script>

<style></style>
