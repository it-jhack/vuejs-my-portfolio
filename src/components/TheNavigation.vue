<template>
  <div>
    <v-navigation-drawer v-model="drawer" app temporary dark>
      <v-divider />

      <v-list dense>
        <v-list-item
          v-for="([icon, text, link], i) in items"
          :key="i"
          link
          @click="$vuetify.goTo(link)"
        >
          <v-list-item-icon class="justify-center">
            <v-icon>{{ icon }}</v-icon>
          </v-list-item-icon>
          <v-list-item-content>
            <v-list-item-title class="subtitile-1 small-text-shadow">
              {{ text }}
            </v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>

    <v-app-bar
      app
      :color="color"
      :flat="flat"
      dark
      class="px-0"
      :class="{ expand: flat }"
    >
      <v-spacer />
      <v-app-bar-nav-icon
        @click.stop="drawer = !drawer"
        class="mr-0"
        v-if="isXs"
      />
      <div v-else>
        <v-btn text @click="$vuetify.goTo(0)">
          <span class="mr-2 small-text-shadow">Home</span>
        </v-btn>
        <v-btn text @click="$vuetify.goTo('#about')">
          <span class="mr-2 small-text-shadow">About</span>
        </v-btn>
        <v-btn text @click="$vuetify.goTo('#projects')">
          <span class="mr-2 small-text-shadow">Projects</span>
        </v-btn>
        <v-btn text @click="$vuetify.goTo('#experience')">
          <span class="mr-2 small-text-shadow">Experience</span>
        </v-btn>
        <v-btn text @click="$vuetify.goTo('#contact')">
          <span class="mr-2 small-text-shadow">Contact</span>
        </v-btn>
      </div>
    </v-app-bar>
  </div>
</template>

<style scoped>
.small-text-shadow {
  color: white;
  text-shadow: 1px 1px 1px #000000;
}

.v-toolbar {
  transition: 0.6s;
}

.expand {
  height: 80px !important;
  padding-top: 10px;
}

.no-anchor-text-decoration {
  text-decoration: none;
}
</style>

<script>
export default {
  data: () => ({
    drawer: null,
    isXs: false,
    items: [
      ["mdi-home-outline", "Home", 0],
      ["mdi-information-outline", "About", "#about"],
      ["mdi-download-box-outline", "Projects", "#projects"],
      ["mdi-briefcase", "Experience", "#experience"],
      ["mdi-email-outline", "Contact", "#contact"],
    ],
  }),
  props: {
    color: String,
    flat: Boolean,
  },
  methods: {
    onResize() {
      this.isXs = window.innerWidth < 850;
    },
  },

  watch: {
    isXs(value) {
      if (!value) {
        if (this.drawer) {
          this.drawer = false;
        }
      }
    },
  },
  mounted() {
    this.onResize();
    window.addEventListener("resize", this.onResize, { passive: true });
  },
};
</script>
