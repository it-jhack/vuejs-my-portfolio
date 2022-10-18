<template>
  <v-footer dark padless>
    <v-card flat tile class="secondary white-text text-center pt-4">
      <v-card-text>
        <v-btn
          v-for="(icon, i) in icons"
          :key="i"
          class="mx-4 white--text"
          :href="icon.link"
          target="_blank"
          icon
        >
          <v-icon size="36px">{{ icon.text }}</v-icon>
        </v-btn>
      </v-card-text>

      <v-card-text class="white--text pt-0">
        <!-- V-card text here -->
      </v-card-text>

      <v-divider></v-divider>

      <v-card-text class="white--text">
        {{ new Date().getFullYear() }} — <strong>Thiago de Paula Amaral</strong>
      </v-card-text>
    </v-card>
  </v-footer>
</template>

<style scoped>
.v-card {
  width: 100%;
}
</style>

<script>
export default {
  data: () => ({
    icons: [
      {
        text: "mdi-github",
        link: "https://github.com/it-jhack",
      },
      {
        text: "mdi-linkedin",
        link: "https://www.linkedin.com/in/thiago-de-paula-amaral/",
      },
    ],
  }),
};
</script>
