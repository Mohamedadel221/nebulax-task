<template>
  <div class="parent-three-cards mt-15">
    <v-container>
      <v-row>
        <v-col
          cols="12"
          md="4"
          sm="4"
          lg="4"
          v-for="cards in threeCards"
          :key="cards.title"
        >
          <v-card>
            <img :src="cards.img" alt="" />
            <v-card-title class="text-uppercase">{{
              cards.title
            }}</v-card-title>
            <v-card-text
              class="text-capitalize"
              v-html="cards.descrip"
            ></v-card-text>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>
<script>
export default {
  data: () => ({
    threeCards: [
      {
        img: require("@/assets/threecards/1.png"),
        title: "fashion store",
        descrip: `shop ladies fashion at missguided <br/> usa with hundreds of new styles <br/> hiting our shelves every weak`,
      },
      {
        img: require("@/assets/threecards/2.png"),
        title: "home furniture",
        descrip: `shop ladies fashion at missguided <br/> usa with hundreds of new styles <br/> hiting our shelves every weak`,
      },
      {
        img: require("@/assets/threecards/1.png"),
        title: "super gadget store",
        descrip: `shop ladies fashion at missguided <br/> usa with hundreds of new styles <br/> hiting our shelves every weak`,
      },
    ],
  }),
};
</script>
<style scoped lang="scss">
.v-card {
  img {
    width: 100%;
    padding: 15px;
  }
  .v-card-text {
    color: #000;
    opacity: 0.4;
  }
}
</style>
