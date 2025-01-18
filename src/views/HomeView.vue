<template>
  <div class="home-page">
    <PhotoandText />
    <LogoPhoto />
    <TextAndTwoPhoto />
    <ThreeCards />
    <CricelSection />
    <WriteUs />
  </div>
</template>

<script>
import PhotoandText from "@/components/HomePage/PhotoandText.vue";
import LogoPhoto from "@/components/HomePage/LogoPhoto.vue";
import TextAndTwoPhoto from "@/components/HomePage/TextAndTwoPhoto.vue";
import ThreeCards from "@/components/HomePage/ThreeCards.vue";
import CricelSection from "@/components/HomePage/CricelSection.vue";
import WriteUs from "@/components/HomePage/WriteUs.vue";
export default {
  name: "HomeView",
  components: {
    PhotoandText,
    LogoPhoto,
    TextAndTwoPhoto,
    ThreeCards,
    CricelSection,
    WriteUs,
  },
};
</script>
