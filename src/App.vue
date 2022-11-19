<template>
  <v-app id="main-app">
    <TheNavigation :color="color" :flat="flat" />
    <v-main class="pt-0">
      <CanvasGreeting />
      <AboutMe id="about" />
      <MyProjects />
      <ExpSection />
      <ContactSection />
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
    <TheFooter />
  </v-app>
</template>

<script>
import TheNavigation from "./components/TheNavigation";
import TheFooter from "./components/TheFooter";
import CanvasGreeting from "@/components/landpage/CanvasGreeting.vue";
import AboutMe from "./components/landpage/AboutMe";
import MyProjects from "./components/landpage/MyProjects";
import ExpSection from "./components/landpage/ExpSection";
import ContactSection from "./components/landpage/ContactSection";

export default {
  name: "App",

  components: {
    TheNavigation,
    TheFooter,
    CanvasGreeting,
    AboutMe,
    MyProjects,
    ExpSection,
    ContactSection,
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
        this.color = "#000000cc";
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

#about {
  margin-top: 100vh;
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

// Webkit Scrollbar
::-webkit-scrollbar {
  width: 5px;
}
::-webkit-scrollbar-track {
  background: #6e6e6e;
}
::-webkit-scrollbar-thumb {
  background: #414141;
}
::-webkit-scrollbar-thumb:hover {
  background: #1f1f1f;
}
</style>
