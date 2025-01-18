<template>
  <div class="parent mt-15">
    <v-container>
      <v-row>
        <v-col cols="12" sm="5" md="4" lg="5">
          <!--text-->
          <div class="text">
            <div class="help">
              <h4 class="text-uppercase mb-2">we help you</h4>
            </div>
            <div class="sell">
              <h1 class="text-capitalize mt-5">
                sell <br />
                stunning <br />
                products
              </h1>
            </div>
            <div class="well-guide">
              <p class="mt-3 mb-0">We'll guide you trough our unique 5-step</p>
              <p class="mt-0 mb-8 left-para position-relative">
                brand-buillding framework
              </p>
            </div>
            <div class="btn mt-5">
              <v-btn
                density="compact"
                width="240"
                height="45"
                color="rgb(131, 58, 200)"
                class="d-flex"
                >more details
                <v-icon size="39">mdi-chevron-right</v-icon></v-btn
              >
            </div>
          </div>
          <!--text-->
        </v-col>
        <v-col cols="12" sm="7" md="6" lg="7">
          <v-row class="align-center">
            <v-col col="6" sm="9" md="7" lg="6">
              <div class="section-chair mt-3">
                <div class="chair-photo mb-2 position-relative">
                  <img
                    class="position-relative"
                    src="@/assets/twophoto/chair.png"
                    alt=""
                  />
                  <div class="minmal-chair">
                    <h5 class="text-capitalize">minimal chair</h5>
                    <v-divider length="75%" color="black"></v-divider>
                  </div>
                  <div
                    class="price-shop-car d-flex justify-space-between align-center"
                  >
                    <h5>$204<span>.00</span></h5>
                    <v-icon size="20">mdi-cart</v-icon>
                  </div>
                </div>
              </div>
              <v-col cols="12" sm="6" md="6" lg="6"> </v-col>
            </v-col>
            <v-col col="6" sm="3" md="5" lg="6">
              <!--section-headphone-->
              <div class="section-headphone position-relative mt-3">
                <div class="headphone-photo mb-2 position-relative">
                  <img
                    class="position-relative"
                    src="@/assets/twophoto/headphones.png"
                    alt=""
                  />
                  <div class="beatsheadphones">
                    <h5 class="text-capitalize">beats headphones</h5>
                    <v-divider length="75%" color="black"></v-divider>
                  </div>
                  <div
                    class="price-shop-car d-flex justify-space-between align-center"
                  >
                    <h5>$74<span>.00</span></h5>
                    <v-icon size="20">mdi-cart</v-icon>
                  </div>
                </div>
              </div>
              <!--section-headphone-->
            </v-col>
          </v-row>
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
    color: #f9dc88;
  }
  h1 {
    font-size: 45px;
  }
  p {
    color: #000 !important;
    opacity: 0.5 !important;
    font-weight: 600;
    white-space: nowrap;
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
      color: rgb(131, 58, 200);
    }
  }
}
/*text-style*/
/*section-chair*/
.section-chair {
  position: relative;
  width: 235px;
  height: 235px;
  border-radius: 50%;
  background-color: #f9dc88;
  margin: auto;
  z-index: 1;
  top: -48px;
  .chair-photo {
    img {
      width: 150px;
      height: 150px;
      display: flex;
      margin: auto;
      align-items: center;
      position: absolute;
      left: 21px;
      top: 37px;
      z-index: 1;
    }
    &::after {
      position: absolute;
      content: "";
      background: #ffffff;
      box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1), 0 1px 3px rgba(0, 0, 0, 0.06);
      border-radius: 8px;
      left: 50px;
      top: 114px;
      width: 73%;
      height: 66%;
      z-index: -1;
    }
  }
  .minmal-chair {
    margin-top: 45px;
    margin-left: 50px;
    text-align: center;
    h5 {
      font-weight: 700;
    }
    .v-divider {
      margin-left: 15px;
      margin-top: 10px;
    }
  }
  .price-shop-car {
    margin-left: 65px;
    width: 140px;
    margin-top: 18px;
    h5 {
      color: rgb(255 191 0 / 96%);
      span {
        color: rgb(255 193 7 / 57%);
      }
    }
  }
}
@media (max-width: 470px) {
  .section-chair {
    top: 0 !important;
  }
}
/*section-chair*/
/*section-chair*/
.section-headphone {
  position: absolute;
  width: 180px;
  height: 180px;
  inset: 0;
  border-radius: 50%;
  background-color: #a99ffb;
  z-index: 1;
  margin-bottom: 123px;
  transform: translate(-11%, 58%);
  .headphone-photo {
    img {
      width: 100%;
      height: 100%;
      display: flex;
      margin: auto;
      align-items: center;
      position: absolute;
      inset: 0;
      transform: translate(-6%, 30%);
      z-index: 1;
    }
    &::after {
      position: absolute;
      content: "";
      background: #ffffff;
      box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1), 0 1px 3px rgba(0, 0, 0, 0.06);
      border-radius: 8px;
      left: 0;
      top: 114px;
      width: 85%;
      height: 66%;
      z-index: -1;
    }
  }
  .beatsheadphones {
    margin-top: 45px;
    margin-right: 33px;
    text-align: center;
    h5 {
      font-weight: 700;
    }
    .v-divider {
      margin-left: 15px;
      margin-top: 10px;
    }
  }
  .price-shop-car {
    margin-left: 17px;
    width: 114px;
    margin-top: 18px;
    h5 {
      color: #f9dc88;
      span {
        color: #f9dc88;
      }
    }
  }
}
@media (max-width: 470px) {
  .section-headphone {
    transform: translate(0%, 0%) !important;
    margin: auto;
  }
}
/*section-chair*/
</style>
