<template>
  <div class="mt-8">
    <div class="logo">
      <v-container fluid>
        <v-row class="align-center">
          <v-col cols="12" md="6" lg="6" sm="6">
            <div class="d-flex justify-center align-center">
              <p class="text-center">Companies we've helped build</p>
            </div>
          </v-col>
          <v-col cols="12" md="6" lg="6" sm="6">
            <div class="d-flex">
              <div v-for="content in image" :key="content.img">
                <img class="w-100" :src="content.img" alt="" />
              </div>
            </div>
          </v-col>
        </v-row>
      </v-container>
    </div>
  </div>
</template>

<script>
export default {
  data: () => ({
    image: [
      {
        img: require("@/assets/img-logos/1.png"),
      },
      {
        img: require("@/assets/img-logos/2.png"),
      },
      {
        img: require("@/assets/img-logos/3.png"),
      },
      {
        img: require("@/assets/img-logos/4.png"),
      },
      {
        img: require("@/assets/img-logos/5.png"),
      },

      {
        title: "Companies we've helped build",
      },
    ],
  }),
};
</script>

<style scoped lang="scss">
.opacity-color {
  color: #000 !important;
  opacity: 0.5 !important;
}
</style>
<!-- v-for="item in image"
:key="item.title" -->
