<template>
  <div class="parent">
    <v-container>
      <v-row class="align-center">
        <v-col cols="12" md="6" sm="12" lg="6">
          <div class="photo">
            <img src="@/assets/cover/cover.png" class="w-100" alt="" />
          </div>
        </v-col>
        <v-col cols="12" md="6" sm="12" lg="6">
          <div class="text">
            <div class="loop-text">
              <h1>We Help You</h1>
              <br />
              <h1>Build & Growth an</h1>
              <br />
              <h1 class="larg-text">Online Business</h1>
            </div>
            <div class="tell-us mt-7 d-flex">
              <div class="input">
                <input
                  type="text"
                  placeholder="Tell us what you need to build"
                />
              </div>
              <div class="icon position-relative">
                <v-icon>mdi-magnify</v-icon>
              </div>
            </div>
          </div>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  data: () => ({}),
};
</script>

<style scoped lang="scss">
.photo {
  img {
    display: flex;
    margin: auto;
  }
}
.text {
  h1 {
    font-size: 50px;
    font-weight: 900;
    font-style: bold;
  }
  .larg-text {
    font-size: 60px;
  }
}
.tell-us {
  input {
    width: 450px;
    border: 2px solid #efefef;
    padding: 10px;
    outline: none;
    border-radius: 5px;
  }
  .v-icon {
    position: absolute;
    right: 10px;
    top: 7.5px;
    color: #fff;
    width: 32.5px;
    height: 32.5px;
    background: rgb(131, 58, 200);
    border-radius: 5px;
    padding: 6px 10px;
  }
}
@media (max-width: 767px) {
  .text {
    h1 {
      font-size: 25px;
    }
  }
  .tell-us {
    input {
      width: 300px;
    }
  }
  .larg-text {
    font-size: 30px !important;
  }
}
@media (min-width: 767px) and (max-width: 1200px) {
  .text {
    h1 {
      font-size: 40px;
    }
  }
}
@media (min-width: 1025px) and (max-width: 1200px) {
  .larg-text {
    font-size: 48px !important;
  }
}
</style>
