<template>
  <section class="pb-8" id="contact">
    <v-container fluid>
      <v-row align="center" justify="center">
        <v-col cols="10">
          <v-row justify="center">
            <v-col cols="12" sm="5" class="v-margin-bottom">
              <h1 class="font-weight-light display-1">/ping my_contact</h1>
              <h3 class="font-weight-light mt-3">
                Contact me and I will be glad to further discuss any related
                topics
              </h3>
              <h3 class="font-weight-light mt-3"></h3>

              <br />
              <v-btn
                class="success no-uppercase"
                href="https://api.whatsapp.com/send?phone=5514998416457"
                target="_blank"
                ><div class="mx-2"><v-icon>mdi-whatsapp</v-icon></div>
                Whatsapp</v-btn
              >
              <br /><br />
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
  background-color: #f4f7f5;
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

<script>
export default {
  data: () => ({
    icons: ["fa-facebook", "fa-twitter", "fa-linkedin", "fa-instagram"],
    valid: true,
  }),
};
</script>
