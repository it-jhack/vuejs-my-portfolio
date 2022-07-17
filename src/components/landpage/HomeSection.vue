<template>
  <section id="home">
    <v-parallax src="@/assets/img/codedesk1.jpg" height="750">
      <v-row align="center" justify="center">
        <v-col cols="10">
          <v-row align="center" justify="center">
            <v-col cols="12" md="6" xl="8">
              <div>
                <h1 class="mb-4 heavy-title">Hi, my name is Thiago</h1>
              </div>
              <div class="home-text">
                <p>
                  I'm an avid self-taught
                  <span class="bold">Full Stack Developer</span>
                  who loves to code and to learn how things work under the hood.
                </p>
                <p>
                  This responsive landing page was created to showcase my
                  portfolio and developing skills.
                </p>
              </div>
              <v-btn
                rounded
                outlined
                large
                dark
                @click="$vuetify.goTo('#about')"
                class="mt-5"
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

<style lang="scss">
section {
  position: relative;
}

.home-text {
  font-size: 24px;
  font-weight: 300;
}
</style>
