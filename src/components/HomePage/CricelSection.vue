<template>
  <div class="parent-cricel mt-8 mb-5">
    <v-container>
      <v-row class="align-center">
        <v-col cols="12" sm="12" md="7" lg="7">
          <v-row>
            <v-col col="12" sm="12" md="12" lg="6">
              <div class="parent-cricel-one">
                <div class="blue-cricel mt-3 position-relative mt-3"></div>
                <div class="box position-relative">
                  <div class="d-flex align-center justify-center">
                    <div class="img">
                      <img
                        class="mr-5"
                        src="@/assets/box-photo/1.jpeg"
                        alt=""
                      />
                    </div>

                    <div class="money text-center">
                      <div
                        class="d-flex align-center justify-center"
                        style="gap: 20px"
                      >
                        <h2>
                          <strong>$ 7,654</strong>
                        </h2>
                        <span>
                          <v-icon size="15" color=""
                            >mdi-chevron-up</v-icon
                          ></span
                        >
                      </div>
                      <p class="text-uppercase">
                        total revenue <span color="green">+$232</span>
                      </p>
                    </div>
                  </div>
                </div>
              </div>
            </v-col>
            <v-col col="12" sm="12" md="12" lg="6">
              <div class="parent-cricel-two">
                <div class="green-circel position-relative mt-3"></div>
                <div class="box position-relative">
                  <div class="d-flex align-center justify-center">
                    <div class="money text-center">
                      <div
                        class="d-flex align-center justify-center"
                        style="gap: 20px"
                      >
                        <span>
                          <v-icon size="15" color=""
                            >mdi-chevron-up</v-icon
                          ></span
                        >
                        <h2>
                          <strong>$ 7,654</strong>
                        </h2>
                      </div>
                      <p class="text-uppercase">
                        total revenue <span>+$232</span>
                      </p>
                    </div>
                    <div class="img">
                      <img
                        class="ml-5"
                        src="@/assets/box-photo/1.jpeg"
                        alt=""
                      />
                    </div>
                  </div>
                </div>
              </div>
            </v-col>
          </v-row>
        </v-col>
        <v-col cols="12" sm="12" md="5" lg="5">
          <!--text-->
          <div class="text">
            <div class="help you">
              <h4 class="text-uppercase mb-2">what we you do</h4>
            </div>
            <div class="sell">
              <h1 class="text-capitalize mt-5">
                increase our <br />
                customers <br />
                sales
              </h1>
            </div>
            <div class="well-guide">
              <p class="mt-3 mb-8">
                We'll guide you trough our unique 5-step <br />
                brand-buillding framework
              </p>
            </div>
            <div class="btn mt-5">
              <v-btn
                density="compact"
                width="240"
                height="45"
                color="#8e42ff"
                class="d-flex"
                >more details
                <v-icon size="39">mdi-chevron-right</v-icon></v-btn
              >
            </div>
          </div>
          <!--text-->
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {};
</script>

<style scoped lang="scss">
/*text-style*/
.text {
  h4 {
    color: rgba(234, 234, 97, 0.867);
  }

  h1 {
    font-size: 45px;
  }

  p {
    color: #000 !important;
    opacity: 0.5 !important;
    font-weight: 600;
  }

  .v-btn {
    font-weight: 700;
    position: relative;
    border-radius: 30px;
    font-size: 16px;

    .v-icon {
      position: absolute;
      right: 2.5px;
      border-radius: 50%;
      background-color: #fff;
      color: #8e42ff;
    }
  }
}

/*text-style*/
/*section-chair*/
.parent-cricel-one {
  .blue-cricel {
    position: relative;
    width: 180px;
    height: 180px;
    border-radius: 50%;
    background-color: #4bb5d8;
    margin: auto;
    z-index: -1;
    top: -48px;
  }
  .box {
    background: #efefef;
    padding: 10px;
    width: 70%;
    border-radius: 10px;
    position: absolute;
    transform: translate(0, -160px);
    span {
      color: #54c883;
    }
  }
  img {
    width: 50px;
    height: 50px;
    border-radius: 50%;
  }
  .money {
    p {
      font-size: 12px;
    }
  }
  .v-icon {
    background-color: #8e42ff;
    border-radius: 50%;
    padding: 5;
    color: #fff;
  }
}
@media (max-width: 767px) {
  .parent-cricel-one {
    trans .box {
      transform: translate(0, -160px) !important;
    }
  }
}
/*section-chair*/
/*section-chair*/

.parent-cricel-two {
  transform: translate(-50%, 91%);
  .green-circel {
    position: relative;
    width: 150px;
    height: 150px;
    border-radius: 50%;
    background-color: #54c883;
    margin: auto;
    z-index: -1;
    top: -48px;
  }
  .box {
    background: #efefef;
    padding: 10px;
    width: 70%;
    border-radius: 10px;
    transform: translate(0, -160px);
    position: absolute;
    span {
      color: #54c883;
    }
    img {
      width: 50px;
      height: 50px;
      border-radius: 50%;
    }
    .money {
      p {
        font-size: 12px;
      }
    }
    .v-icon {
      background-color: #8e42ff;
      border-radius: 50%;
      padding: 5;
      color: #fff;
    }
  }
}
@media (max-width: 1024px) {
  .parent-cricel-two {
    transform: translate(0px, 0) !important;
    .box {
      transform: translate(0, -160px) !important;
    }
  }
}
/*section-chair*/
</style>
