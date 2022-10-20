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
                <p>
                  Make sure to check out my Projects and Gists on GitHub
                  @it-jhack
                </p>
                <v-btn
                  rounded
                  outlined
                  href="https://github.com/it-jhack"
                  target="_blank"
                  large
                  color="white"
                  class="mt-2"
                >
                  <v-icon class="mr-2">mdi-github</v-icon>
                  GitHub
                </v-btn>

                <p class="mt-5">Check out some of my public projects:</p>

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
                </v-tooltip>
              </div>
            </v-col>

            <v-col sm="6" class="hidden-xs-only">
              <v-img
                contain
                src="@/assets/img/project-movie-title-translator.gif"
                position="top"
                class="project-img"
              />
              <v-img
                contain
                src="@/assets/img/project-swapi.gif"
                position="top"
                class="project-img"
              />
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
    return {};
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
