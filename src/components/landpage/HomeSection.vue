<template>
  <section id="home">
    <v-parallax src="@/assets/img/codedesk1.jpg" height="750">
      <v-row align="center" justify="center">
        <v-col cols="10">
          <v-row align="center" justify="center">
            <v-col cols="12" md="6" xl="8">
              <h1 class="display-2 font-weight-bold mb-4 large-text-shadow">
                Hi, my name is Thiago
              </h1>
              <h1 class="font-weight-light small-text-shadow">
                <p>
                  I'm an avid self-taught programmer who loves to code and to
                  learn how stuff works.
                </p>
                <p>
                  This responsive landing page was created to showcase my
                  portfolio and developing skills.
                </p>
              </h1>
              <v-btn
                rounded
                outlined
                large
                dark
                @click="$vuetify.goTo('#about')"
                class="mt-5 small-text-shadow"
              >
                Tell me more
                <v-icon class="ml-2">mdi-arrow-down</v-icon>
              </v-btn>
            </v-col>
            <v-col cols="12" md="6" xl="4" class="hidden-sm-and-down"> </v-col>
          </v-row>
        </v-col>
      </v-row>
    </v-parallax>
  </section>
</template>

<script>
export default {
  data() {
    return {
      dialog: false,
    };
  },
  watch: {
    dialog(value) {
      if (!value) {
        this.pause();
      }
    },
  },
};
</script>

<style>
section {
  position: relative;
}
</style>
