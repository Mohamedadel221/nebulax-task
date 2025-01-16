<template>
  <div class="home-page">
    <PhotoandText />
    <LogoPhoto />
    <TextAndTwoPhoto />
  </div>
</template>

<script>
import PhotoandText from "@/components/HomePage/PhotoandText.vue";
import LogoPhoto from "@/components/HomePage/LogoPhoto.vue";
import TextAndTwoPhoto from "@/components/HomePage/TextAndTwoPhoto.vue";
export default {
  name: "HomeView",
  components: {
    PhotoandText,
    LogoPhoto,
    TextAndTwoPhoto,
  },
};
</script>
