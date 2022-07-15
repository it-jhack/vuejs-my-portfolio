<template>
  <section id="projects">
    <v-container fluid>
      <v-row align="center" justify="center">
        <v-col cols="10">
          <v-row class="mt-5">
            <v-col cols="12" sm="6" class="text-left">
              <h1 class="font-weight-light white-color display-2 mb-2">
                /git clone projects.git
              </h1>
              <h1 class="font-weight-light white-color">
                Make sure to checkout my Projects and Gists on GitHub
                @it-jhack<br />
                <v-btn
                  rounded
                  outlined
                  href="https://github.com/it-jhack"
                  target="_blank"
                  large
                  color="white"
                  class="mt-5"
                >
                  <v-icon class="mr-2"> mdi-github </v-icon>
                  GitHub
                </v-btn>

                <p class="mt-5">Checkout some of my public projects:</p>

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
                    Project I did mid 2021 uniting front-end and back-end. The
                    front-end fetches characters from Star Wars Api (Swapi),
                    processes the response JSON object and returns which Star
                    Wars movies the selected character has been in. If available
                    as an environment variable it also uses Bing search engine
                    to search for the character and shows the first image result
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
                    Python to help find Subdomain Takeover vulnerabilities
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
                    <p class="my-0">
                      <a
                        href="https://github.com/it-jhack/subsort"
                        target="_blank"
                      >
                        /subsort
                        <v-icon class="info-icon" v-bind="attrs" v-on="on">
                          mdi-information-outline
                        </v-icon>
                      </a>
                    </p>
                  </template>
                  <span>
                    An algorithm I developed in Python, as part of the Subtaker
                    project, that removes subdomain redundancies and returns an
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
                    <p class="my-0">
                      <a
                        href="https://github.com/it-jhack/bughunter-debian-setup"
                        target="_blank"
                      >
                        /bughunter-setup
                        <v-icon class="info-icon" v-bind="attrs" v-on="on">
                          mdi-information-outline
                        </v-icon>
                      </a>
                    </p>
                  </template>
                  <span>
                    A Bash script (linux programming language) I created to
                    install essential tools for Bug Bounty Hunters on a fresh
                    Debian Operational System.
                  </span>
                </v-tooltip>
              </h1>
            </v-col>

            <v-col sm="6" class="hidden-xs-only">
              <v-dialog
                v-model="swapiDialog"
                max-width="65vw"
                class="m-10"
                dark
              >
                <template v-slot:activator="{ on, attrs }">
                  <a>
                    <v-img
                      v-bind="attrs"
                      v-on="on"
                      contain
                      src="@/assets/img/swapi-demo.gif"
                      position="top"
                      class="mt-2 mb-4"
                    />
                  </a>
                </template>

                <v-card>
                  <v-img
                    class="d-flex justify-center"
                    v-bind="attrs"
                    v-on="on"
                    contain
                    src="@/assets/img/swapi-demo.gif"
                    position="top"
                    
                    max-width="65vw"
                    max-height="80vh"
                  />
                </v-card>
              </v-dialog>
            </v-col>
          </v-row>
        </v-col>
      </v-row>
    </v-container>
  </section>
</template>

<script>
  export default {
    data () {
      return {
        swapiDialog: false,
      }
    },
  }
</script>

<style scoped>
#projects {
  background-image: url("~@/assets/img/bgDownload.jpg");
  background-attachment: fixed;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  height: 600px;
}

#projects .container,
#projects .row {
  height: 100%;
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
</style>
