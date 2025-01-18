<template>
  <div class="parent-why-us mt-15">
    <v-container>
      <v-row>
        <v-col cols="12" md="6" sm="12" lg="6">
          <v-card
            style="border-radius: 8px"
            height="100%"
            class="d-flex justify-center align-center"
          >
            <div class="section-form">
              <div class="box text-center">
                <h2 class="mb-3 text-capitalize">write us</h2>
                <div
                  class="inputs d-flex justify-center align-center mb-5 position-relative"
                >
                  <v-icon
                    v-if="!emailFocused && !emailValue"
                    size="15"
                    class="position-relative"
                  >
                    mdi-email
                  </v-icon>
                  <input
                    type="text"
                    placeholder="morad.blil@gmail.com"
                    v-model="emailValue"
                    @focus="emailFocused = true"
                    @blur="checkEmailFocus"
                  />
                </div>
                <div
                  class="text-area d-flex justify-center align-center position-relative"
                >
                  <v-icon
                    v-if="!messageFocused && !messageValue"
                    size="15"
                    class="position-relative"
                  >
                    mdi-mail
                  </v-icon>
                  <textarea
                    placeholder="Enter your message"
                    v-model="messageValue"
                    @focus="messageFocused = true"
                    @blur="checkMessageFocus"
                  ></textarea>
                </div>
                <div
                  class="btn-send-mesage mt-5 d-flex justify-center align-center"
                >
                  <v-btn
                    density="compact"
                    width="240"
                    height="45"
                    color="#8e42ff"
                    class="d-flex"
                    style="
                      border-radius: 30px;
                      font-weight: 700;
                      font-size: 16px;
                    "
                    >send message
                  </v-btn>
                </div>
              </div>
            </div>
          </v-card>
        </v-col>
        <v-col cols="12" md="6" sm="12" lg="6">
          <img class="w-100 h-100" src="@/assets/write-us/why-us.png" alt="" />
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>
<script>
export default {
  data: () => ({
    emailFocused: false,
    emailValue: "",
    messageFocused: false,
    messageValue: "",
  }),
  methods: {
    checkEmailFocus() {
      if (!this.emailValue) {
        this.emailFocused = false;
      }
    },
  },
  checkMessageFocus() {
    if (!this.messageValue) {
      this.messageFocused = false;
    }
  },
};
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
@media (max-width: 1200px) {
  .v-card {
    padding: 80px;
  }
}
@media (max-width: 591px) {
  input,
  textarea {
    width: 300px;
  }
}
</style>
