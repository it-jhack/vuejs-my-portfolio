<template>
  <div>
    <canvas ref="canvas" />
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
canvas {
  width: 100vw;
  height: 100vh;
}
</style>
