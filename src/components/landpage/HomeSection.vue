<template>
  <section id="home">
    <v-parallax
      v-if="!$store.state.isMobile"
      src="@/assets/img/codedesk1.jpg"
      height="750"
    >
      <HomeContent />
    </v-parallax>
    <div v-else class="mobile-home-bg">
      <HomeContent />
    </div>
  </section>
</template>

<script>
import HomeContent from "@/components/landpage/HomeContent.vue";

export default {
  components: {
    HomeContent,
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
  color: white;
}

.mobile-home-bg {
  padding-top: 6rem;
  padding-bottom: 3rem;
  position: relative;
  background-image: url("~@/assets/img/codedesk1.jpg");
  background-position: center;
  background-size: cover;
  background-color: #292929;
}
</style>
