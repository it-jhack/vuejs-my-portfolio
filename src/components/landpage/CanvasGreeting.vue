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
              <span class="bold">Front-end Developer</span>
              who loves to code and learn how things work.
            </p>
            <p>
              This responsive landing page was created to showcase my portfolio
              and coding skills.
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

    // Edit canvas WebGL Fluid Simulation Properties: see more at https://www.npmjs.com/package/webgl-fluid
    // WebGLFluid(document.querySelector('canvas'), {
    //   IMMEDIATE: true, // Whether to trigger multiple random splats when initialized
    //   TRIGGER: 'hover', // Can be change to 'click'
    //   SIM_RESOLUTION: 128,
    //   DYE_RESOLUTION: 1024,
    //   CAPTURE_RESOLUTION: 512,
    //   DENSITY_DISSIPATION: 1,
    //   VELOCITY_DISSIPATION: 0.2,
    //   PRESSURE: 0.8,
    //   PRESSURE_ITERATIONS: 20,
    //   CURL: 30,
    //   SPLAT_RADIUS: 0.25,
    //   SPLAT_FORCE: 6000,
    //   SHADING: true,
    //   COLORFUL: true,
    //   COLOR_UPDATE_SPEED: 10,
    //   PAUSED: false,
    //   BACK_COLOR: { r: 0, g: 0, b: 0 },
    //   TRANSPARENT: false,
    //   BLOOM: true,
    //   BLOOM_ITERATIONS: 8,
    //   BLOOM_RESOLUTION: 256,
    //   BLOOM_INTENSITY: 0.8,
    //   BLOOM_THRESHOLD: 0.6,
    //   BLOOM_SOFT_KNEE: 0.7,
    //   SUNRAYS: true,
    //   SUNRAYS_RESOLUTION: 196,
    //   SUNRAYS_WEIGHT: 0.75,
    // })
  },
};
</script>

<style lang="scss" scoped>
@media (max-width: 320px) {
  .greeting-margin {
    margin-top: -20vh !important;
    margin-left: 2vw !important;
  }
  .heavy-title {
    font-size: 28px !important;
    font-weight: 500 !important;
  }
  .greeting-text {
    font-size: 18px !important;
  }
}

@media (min-width: 321px) and (max-width: 360px) {
  .greeting-margin {
    margin-top: -20vh !important;
    margin-left: 2vw !important;
  }
  .heavy-title {
    font-size: 36px !important;
    font-weight: 500 !important;
  }
  .greeting-text {
    font-size: 22px !important;
  }
}

@media (min-width: 361px) and (max-width: 384px) {
  .greeting-margin {
    margin-top: -10vh !important;
    margin-left: 2vw !important;
  }
  .heavy-title {
    font-size: 36px !important;
    font-weight: 500 !important;
  }
  .greeting-text {
    font-size: 22px !important;
  }
}

@media (min-width: 361px) and (max-width: 450px) {
  .greeting-margin {
    margin-top: -18vh !important;
    margin-left: 2vw !important;
  }
}

@media (min-width: 450px) and (max-width: 768px) {
  #greeting {
    margin-top: 13vh !important;
  }

  .greeting-margin {
    margin-left: 2vw !important;
  }
}

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
