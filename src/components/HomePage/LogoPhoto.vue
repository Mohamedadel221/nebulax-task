<template>
  <div class="mt-2">
    <div class="logo">
      <v-container>
        <div>
          <v-row class="align-center">
            <v-col col="12" md="4" lg="4">
              <div class="text-center" v-for="item in image" :key="item.title">
                <h4 class="text-center opacity-color">{{ item.title }}</h4>
              </div>
            </v-col>
            <v-col
              class="d-flex justify-space-between align-center"
              col="12"
              md="2"
              lg="2"
              v-for="item in image"
              :key="item.title"
            >
              <div class="logo">
                <img
                  :src="item.img"
                  style="width: 150px"
                  class=""
                  alt=""
                /></div
            ></v-col>
          </v-row>
        </div>
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
