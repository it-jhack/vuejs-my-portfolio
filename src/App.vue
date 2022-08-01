<template>
  <v-app id="main-app">
    <navigation :color="color" :flat="flat" />
    <v-main class="pt-0">
      <WebglFluidSim />
      <!-- <home /> -->
      <about style="margin-top: 100vh;" />
      <projects />
      <experience />
      <contact />
    </v-main>
    <v-scale-transition v-if="!$store.state.isMobile">
      <v-btn
        fab
        v-show="fab"
        v-scroll="onScroll"
        dark
        fixed
        bottom
        right
        color="secondary"
        @click="toTop"
      >
        <v-icon>mdi-arrow-up</v-icon>
      </v-btn>
    </v-scale-transition>
    <myfooter />
  </v-app>
</template>

<script>
import WebglFluidSim from "@/components/landpage/WebglFluidSim.vue";
import navigation from "./components/Navigation";
import myfooter from "./components/Footer";
// import home from "./components/landpage/HomeSection";
import about from "./components/landpage/AboutMe";
import projects from "./components/landpage/Projects";
import experience from "./components/landpage/ExpSection";
import contact from "./components/landpage/ContactSection";

export default {
  name: "App",

  components: {
    navigation,
    myfooter,
    WebglFluidSim,
    // home,
    about,
    projects,
    experience,
    contact,
  },

  data: () => ({
    fab: null,
    color: "",
    flat: null,
  }),

  created() {
    const top = window.pageYOffset || 0;
    if (top <= 30) {
      this.color = "transparent";
      this.flat = true;
    }
  },

  watch: {
    fab(value) {
      if (value) {
        this.color = "secondary";
        this.flat = false;
      } else {
        this.color = "transparent";
        this.flat = true;
      }
    },
  },

  methods: {
    onScroll(e) {
      setTimeout(() => {
        if (typeof window === "undefined") return;
        const top = window.pageYOffset || e.target.scrollTop || 0;
        this.fab = top > 30;
      }, 125);
    },
    toTop() {
      this.$vuetify.goTo(0);
    },
  },
};
</script>

<style scoped>
#main-app {
  overflow-x: hidden !important;
  background-color: #02000d !important;
}
</style>

<style lang="scss">
/* Global classes */

.d-flex {
  display: flex;
}

.text-align-justify {
  text-align: justify;
}

.justify-content-space-evenly {
  justify-content: space-evenly;
}

.white-color {
  color: #ffffff;
}

.bold {
  font-weight: 500;
}

.heavy-title {
  font-size: 48px;
  font-weight: 700;
}

.p-text {
  font-size: 22px;
  font-weight: 300;
}

.terminal-title {
  color: #ffffff;
  font-family: Roboto Mono !important;
  font-weight: 500;
  font-size: 40px;
  line-height: 1em;
}

.terminal-title::after {
  content: "_";
  -webkit-animation: blink 1s step-end infinite;
  animation: blink 1s step-end infinite;
}

@-webkit-keyframes blink {
  0% {
    opacity: 1;
  }
  50% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}

@keyframes blink {
  0% {
    opacity: 1;
  }
  50% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}
</style>
