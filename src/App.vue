<template>
  <v-app>
    <navigation :color="color" :flat="flat" />
    <v-main class="pt-0">
      <home />
      <about />
      <projects class="mb-3" />
      <experience />
      <contact />
    </v-main>
    <myfooter />
  </v-app>
</template>

<script>
import navigation from "./components/Navigation";
import myfooter from "./components/Footer";
import home from "./components/landpage/HomeSection";
import about from "./components/landpage/AboutMe";
import projects from "./components/landpage/Projects";
import experience from "./components/landpage/ExpSection";
import contact from "./components/landpage/ContactSection";

export default {
  name: "App",

  components: {
    navigation,
    myfooter,
    home,
    about,
    projects,
    experience,
    contact,
  },
};
</script>

<style scoped>
.v-main {
  background-image: url("~@/assets/img/bgMain.png");
  background-attachment: fixed;
  background-position: center;
  background-size: cover;
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
