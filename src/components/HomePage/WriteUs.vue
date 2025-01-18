<template>
  <div class="parent-why-us mt-15 mb-5">
    <v-container>
      <v-row>
        <v-col cols="12" md="6" sm="12" lg="6">
          <v-card height="100%" class="d-flex justify-center align-center">
            <div class="section-form">
              <div class="box text-center">
                <h2 class="mb-3 text-capitalize">write us</h2>
                <div
                  class="inputs d-flex justify-center align-center mb-5 position-relative"
                >
                  <v-icon size="15" class="position-relative">mdi-email</v-icon>
                  <input type="text" placeholder="morad.blil@gmail.com" />
                </div>
                <div
                  class="text-area d-flex justify-center align-center position-relative"
                >
                  <v-icon size="15" class="position-relative">mdi-mail</v-icon>
                  <textarea
                    name=""
                    placeholder="Enter your message"
                    id=""
                  ></textarea>
                </div>
              </div>
            </div>
          </v-card>
        </v-col>
        <v-col cols="12" md="6" sm="12" lg="6">
          <img class="w-100" src="@/assets/write-us/why-us.png" alt="" />
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>
<script>
export default {};
</script>
<style scoped lang="scss">
.box {
  background: #ffffff;
  height: 100%;
  .inputs {
    input {
      border-radius: 30px;
      width: 400px;
      outline: none;
      background: #efefef;
      padding: 10px;
    }
    .v-icon {
      position: absolute;
      right: -39px;
      color: #000;
      top: 0px;
      opacity: 0.5;
    }
    input::placeholder {
      color: #000;
      padding-left: 35px;
    }
  }
  .text-area {
    textarea {
      border-radius: 30px;
      width: 400px;
      outline: none;
      background: #efefef;
      padding: 10px;
      height: 170px;
    }
    textarea::placeholder {
      padding-left: 35px;
    }
    .v-icon {
      position: absolute;
      right: -39px;
      top: -62px;
      color: #000;
      opacity: 0.5;
    }
  }
}
</style>
