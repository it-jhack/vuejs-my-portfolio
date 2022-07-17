<template>
  <section class="pb-8" id="contact">
    <v-container fluid>
      <v-row align="center" justify="center">
        <v-col cols="10">
          <v-row justify="center">
            <v-col cols="12" sm="5" class="v-margin-bottom">
              <div class="terminal-title mt-5">/ssh my_contact</div>
              <div class="p-text white-color mt-8 text-align-justify">
                Contact me and I will be glad to further discuss any related
                topics                
              </div>
            </v-col>
          </v-row>
          <v-row>
            <v-col align="center">
              <v-btn
                class="mt-5 mb-5"
                color="#299e55"
                href="https://api.whatsapp.com/send?phone=5514998416457"
                target="_blank"
              >
                <v-icon class="white-color" style="color: white">mdi-whatsapp</v-icon>
                <span class="white-color">Whatsapp</span>
              </v-btn>
            </v-col>
          </v-row>
        </v-col>
      </v-row>
    </v-container>
    <div class="svg-border-waves text-white">
      <v-img src="~@/assets/img/borderWavesBlue.svg" />
    </div>
  </section>
</template>

<style scoped>
#contact {
  background-color: #00010f;
}

.svg-border-waves .v-image {
  position: absolute;
  bottom: 0;
  left: 0;
  height: 3rem;
  width: 100%;
  overflow: hidden;
}
</style>
