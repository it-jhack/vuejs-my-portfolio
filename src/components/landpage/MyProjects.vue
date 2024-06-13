<template>
  <section
    id="projects"
    class="pb-3 mb-xl-12"
    :class="$store.state.isMobile ? 'mobile-bg' : 'desktop-bg'"
  >
    <v-container fluid>
      <v-row align="center" justify="center">
        <v-col cols="10">
          <v-row class="mt-5">
            <v-col cols="12" sm="6" class="text-left">
              <p class="terminal-title mb-2">/git clone projects.git</p>
              <div class="p-text white-color mt-5">
                <p>Check out my projects on GitHub @it-jhack</p>

                <v-btn
                  rounded
                  outlined
                  href="https://github.com/it-jhack"
                  target="_blank"
                  large
                  color="white"
                  class="mt-2 mr-3"
                >
                  <v-icon class="mr-2">mdi-github</v-icon>
                  GitHub
                </v-btn>

                <v-dialog
                  v-if="this.$store.state.isMobile"
                  overlay-color="black"
                  v-model="githubStatsDialog"
                  max-width="290"
                >
                  <template v-slot:activator="{ on, attrs }">
                    <v-btn
                      v-bind="attrs"
                      v-on="on"
                      rounded
                      outlined
                      large
                      color="white"
                      class="mt-2"
                    >
                      <v-icon class="mr-2">mdi-star-outline</v-icon>
                      Stats
                    </v-btn>
                  </template>
                  <v-card dark>
                    <v-card-text class="pt-5">
                      <p class="p-text white-color">My Github Stats</p>
                      <img
                        class="github-stats-cards"
                        src="https://github-readme-stats.vercel.app/api?username=it-jhack&show_icons=true&bg_color=1f222e&hide_border=1&title_color=42b883&theme=gotham&hide_rank=true"
                      />

                      <p class="p-text white-color mt-5">
                        Open-source projects I've contributed to
                      </p>
                      <p>
                        <a
                          href="https://github.com/DenverCoder1/readme-typing-svg/pull/165"
                          target="_blank"
                        >
                          <img
                            class="github-stats-cards"
                            src="https://denvercoder1-github-readme-stats.vercel.app/api/pin/?username=DenverCoder1&repo=readme-typing-svg&theme=react&bg_color=1f222e&title_color=42b883&hide_border=true&icon_color=f8d866"
                          />
                        </a>
                      </p>
                    </v-card-text>
                    <v-card-actions>
                      <v-spacer></v-spacer>
                      <v-btn
                        color="darken-1"
                        text
                        @click="githubStatsDialog = false"
                      >
                        Close
                      </v-btn>
                    </v-card-actions>
                  </v-card>
                </v-dialog>

                <!-- <p class="mt-5">Check out some of my public projects:</p>

                <v-tooltip
                  :bottom="!this.$store.state.isMobile"
                  :top="this.$store.state.isMobile"
                  :nudge-top="!this.$store.state.isMobile ? '42' : ''"
                  :nudge-right="!this.$store.state.isMobile ? '130' : ''"
                  :max-width="!this.$store.state.isMobile ? '20vw' : '90vw'"
                >
                  <template v-slot:activator="{ on, attrs }">
                    <div class="my-0">
                      <a
                        href="https://github.com/it-jhack/vuejs-my-portfolio"
                        target="_blank"
                      >
                        /vuejs-my-portfolio
                      </a>
                      <v-icon class="info-icon" v-bind="attrs" v-on="on">
                        mdi-information-outline
                      </v-icon>
                    </div>
                  </template>
                  <span>
                    The project of this very portfolio site you're seeing.
                  </span>
                </v-tooltip>

                <v-tooltip
                  :bottom="!this.$store.state.isMobile"
                  :top="this.$store.state.isMobile"
                  :nudge-top="!this.$store.state.isMobile ? '42' : ''"
                  :nudge-right="!this.$store.state.isMobile ? '130' : ''"
                  :max-width="!this.$store.state.isMobile ? '20vw' : '90vw'"
                >
                  <template v-slot:activator="{ on, attrs }">
                    <div class="my-0">
                      <a
                        href="https://github.com/it-jhack/movie-title-translator"
                        target="_blank"
                      >
                        /movie-title-translator
                      </a>
                      <v-icon class="info-icon" v-bind="attrs" v-on="on">
                        mdi-information-outline
                      </v-icon>
                    </div>
                  </template>
                  <span>
                    The Movie Title Translator is a project I made purely to
                    learn and experiment with React and Next.js (coming from a
                    Vue.js background as a developer).
                  </span>
                </v-tooltip>

                <v-tooltip
                  :bottom="!this.$store.state.isMobile"
                  :top="this.$store.state.isMobile"
                  :nudge-top="!this.$store.state.isMobile ? '42' : ''"
                  :nudge-right="!this.$store.state.isMobile ? '130' : ''"
                  :max-width="!this.$store.state.isMobile ? '20vw' : '90vw'"
                >
                  <template v-slot:activator="{ on, attrs }">
                    <div class="my-0">
                      <a
                        href="https://github.com/it-jhack/vuejs-swapi"
                        target="_blank"
                      >
                        /swapi
                        <span class="white-color item-parenthesis">
                          (Star Wars API)
                        </span>
                      </a>
                      <v-icon class="info-icon" v-bind="attrs" v-on="on">
                        mdi-information-outline
                      </v-icon>
                    </div>
                  </template>
                  <span>
                    Project I did mid-2021. The front-end fetches characters
                    from Star Wars Api (Swapi), processes the response JSON
                    object and returns which movies the selected character has
                    been in. If you provide an appropriate secret key for Bing
                    Search Engine as an environment variable, it will also
                    display the first image result for each character
                  </span>
                </v-tooltip>

                <v-tooltip
                  :bottom="!this.$store.state.isMobile"
                  :top="this.$store.state.isMobile"
                  :nudge-top="!this.$store.state.isMobile ? '42' : ''"
                  :nudge-right="!this.$store.state.isMobile ? '130' : ''"
                  :max-width="!this.$store.state.isMobile ? '20vw' : '90vw'"
                >
                  <template v-slot:activator="{ on, attrs }">
                    <div class="my-0">
                      <a
                        href="https://github.com/it-jhack/subtaker"
                        target="_blank"
                      >
                        /subtaker
                      </a>
                      <v-icon class="info-icon" v-bind="attrs" v-on="on">
                        mdi-information-outline
                      </v-icon>
                    </div>
                  </template>
                  <span>
                    Subtaker is a security penetration tool I developed in
                    Python to help find 'Subdomain Takeover' vulnerabilities
                  </span>
                </v-tooltip>

                <v-tooltip
                  :bottom="!this.$store.state.isMobile"
                  :top="this.$store.state.isMobile"
                  :nudge-top="!this.$store.state.isMobile ? '42' : ''"
                  :nudge-right="!this.$store.state.isMobile ? '130' : ''"
                  :max-width="!this.$store.state.isMobile ? '20vw' : '90vw'"
                >
                  <template v-slot:activator="{ on, attrs }">
                    <div class="my-0">
                      <a
                        href="https://github.com/it-jhack/subsort"
                        target="_blank"
                      >
                        /subsort
                      </a>
                      <v-icon class="info-icon" v-bind="attrs" v-on="on">
                        mdi-information-outline
                      </v-icon>
                    </div>
                  </template>
                  <span>
                    An algorithm I developed in Python, as part of the Subtaker
                    project. It removes subdomain redundancies and returns an
                    optimized list. It saves a lot of time and computing
                    resources when parsing through large subdomain/DNS database
                    files
                  </span>
                </v-tooltip>

                <v-tooltip
                  :bottom="!this.$store.state.isMobile"
                  :top="this.$store.state.isMobile"
                  :nudge-top="!this.$store.state.isMobile ? '42' : ''"
                  :nudge-right="!this.$store.state.isMobile ? '130' : ''"
                  :max-width="!this.$store.state.isMobile ? '20vw' : '90vw'"
                >
                  <template v-slot:activator="{ on, attrs }">
                    <div class="my-0">
                      <a
                        href="https://github.com/it-jhack/bughunter-debian-setup"
                        target="_blank"
                      >
                        /bughunter-setup
                      </a>
                      <v-icon class="info-icon" v-bind="attrs" v-on="on">
                        mdi-information-outline
                      </v-icon>
                    </div>
                  </template>
                  <span>
                    A terminal Bash Script (programming in Linux) that I created
                    to automate the installation of essential tools for Bug
                    Bounty Hunters on a fresh Debian Operational System.
                  </span>
                </v-tooltip> -->
              </div>
            </v-col>

            <v-col v-if="!this.$store.state.isMobile" sm="6">
              <img
                src="https://github-readme-stats.vercel.app/api?username=it-jhack&show_icons=true&bg_color=1f222e&hide_border=1&title_color=42b883&theme=gotham"
              />

              <p class="p-text white-color mt-5">
                Open-source projects I've contributed to
              </p>
              <p>
                <a
                  href="https://github.com/DenverCoder1/readme-typing-svg/pull/165"
                  target="_blank"
                >
                  <img
                    src="https://denvercoder1-github-readme-stats.vercel.app/api/pin/?username=DenverCoder1&repo=readme-typing-svg&theme=react&bg_color=1f222e&title_color=42b883&hide_border=true&icon_color=f8d866"
                  />
                </a>
              </p>
            </v-col>
          </v-row>
        </v-col>
      </v-row>
    </v-container>
  </section>
</template>

<script>
export default {
  data() {
    return {
      githubStatsDialog: false,
    };
  },
};
</script>

<style lang="scss" scoped>
#projects {
  height: 600px;
}

#projects .container,
#projects .row {
  height: 100%;
}

.desktop-bg {
  background-image: url("~@/assets/img/codedesk1.jpg");
  background-size: cover;
  background-position: center;
  background-attachment: fixed;
  background-repeat: no-repeat;
}

.mobile-bg {
  background-color: #02000d;
  min-height: 85vh;
}

.rounded-corners {
  border-radius: 20%;
}

.github-stats-cards {
  max-width: 67.5vw;
}

.info-icon {
  color: white !important;
}

a {
  color: #56f031 !important;
  text-decoration: none;
}

a:visited {
  color: #56f031;
  text-decoration: none;
}

.item-parenthesis {
  font-size: 18px;
}

.v-tooltip__content {
  opacity: 1 !important;
  background: #292929;
}

.project-img {
  height: 250px;
  width: 445px;
  margin: 0 0 20px 0;
}
</style>
