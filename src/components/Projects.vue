<template>
  <section id="projects">
    <v-container fluid>
      <v-row align="center" justify="center">
        <v-col cols="10">
          <v-row align="center" justify="center">
            <v-col cols="12" sm="6" class="white--text text-left">
              <h1 class="font-weight-light display-2 mb-2">
                /git clone projects.git
              </h1>
              <h1 class="font-weight-light">
                Make sure to checkout my Projects and Gists on GitHub
                @it-jhack<br />
                <v-btn
                  rounded
                  outlined
                  href="https://github.com/it-jhack"
                  target="_blank"
                  large
                  color="white"
                  class="mt-4"
                >
                  <v-icon class="mr-2"> mdi-github </v-icon>
                  Git Hub
                </v-btn>
                <br /><br />
                Checkout some of my public projects: <br />
                <a
                  class="green-text"
                  href="https://github.com/it-jhack/subtaker"
                  target="_blank"
                  >/subtaker</a
                ><br />
                <a
                  class="green-text"
                  href="https://github.com/it-jhack/subsort"
                  target="_blank"
                  >/subsort</a
                ><br />
                <a
                  class="green-text"
                  href="https://github.com/it-jhack/bughunter-debian-setup"
                  target="_blank"
                  >/bughunter-debian-setup</a
                ><br />
              </h1>
            </v-col>

            <v-col sm="6" class="hidden-xs-only">
              <v-img
                src="@/assets/img/subtaker.png"
                contain="true"
                position="top center"
              />
            </v-col>
          </v-row>
        </v-col>
      </v-row>
      <!-- #!DELETE? -->
      <div class="svg-border-waves text-white">
        <v-img src="@/assets/img/borderWaves.svg" />
      </div>
    </v-container>
  </section>
</template>

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

.green-text {
  color: #56f031;
  text-decoration: none;
}

a:visited {
  color: #56f031;
  text-decoration: none;
}
</style>
