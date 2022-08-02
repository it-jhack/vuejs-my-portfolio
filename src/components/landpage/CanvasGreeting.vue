<template>
  <div id="canvas-greeting">
    <canvas ref="canvas" />

    <v-col id="greeting" sm="10" md="8" lg="6" xl="4">
      <v-col>
        <v-col class="greeting-margin">
          <div>
            <h1 class="mb-4 heavy-title white-color">Hi, my name is Thiago</h1>
          </div>
          <div class="greeting-text white-color">
            <p>
              I'm an avid self-taught
              <span class="bold">Full Stack Developer</span>
              who loves to code and to learn how things work.
            </p>
            <p>
              This responsive landing page was created to showcase my portfolio
              and code developing skills.
            </p>
          </div>
          <v-btn
            id="go-to-about"
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
      </v-col>
    </v-col>
  </div>
</template>

<script>
import WebGLFluid from "webgl-fluid";

export default {
  mounted() {
    WebGLFluid(this.$refs.canvas);
  },
};
</script>

<style scoped>
#canvas-greeting {
  position: relative;
}

canvas {
  position: absolute;
}

#greeting {
  position: absolute;
  margin-top: 25vh;
  pointer-events: none;
  text-shadow: 1px 1px 1px #000000;
}

canvas {
  width: 100vw;
  height: 100vh;
}

.v-btn {
  pointer-events: auto !important;
  text-shadow: 1px 1px 1px #000000;
}

.greeting-text {
  font-size: 24px;
  font-weight: 300;
}

.greeting-margin {
  margin-left: 8vw;
}
</style>
