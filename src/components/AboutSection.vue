<template>
  <section id="about">
    <v-container fluid>
      <v-row align="center" justify="center">
        <v-col cols="10">
          <v-row align="center" justify="center">
            <v-col sm="4" class="hidden-xs-only">
              <v-img
                src="@/assets/img/thiago.jpg"
                class="d-block ml-auto mr-auto"
                max-width="200px"
              />
            </v-col>
            <v-col cols="12" sm="8" class="white--text text-left">
              <h1 class="font-weight-light display-2 mb-2">/whoami</h1>
              <h1 class="font-weight-light">
                My name is Thiago Amaral, I'm a Systems Analysis and Development
                student from Brazil, although most of what I know I learned by
                myself online.
              </h1>
              <br />
              <h1 class="font-weight-light">
                I love to code and to learn programming and networking by
                building small projects. I also have an Engineering degree.
              </h1>
              <v-btn
                rounded
                outlined
                href="https://github.com/Joabsonlg/Landing-Page"
                target="_blank"
                large
                color="white"
                class="mt-4"
              >
                <v-icon class="mr-2"> mdi-github </v-icon>
                Git Hub
              </v-btn>
            </v-col>
          </v-row>
        </v-col>
      </v-row>
    </v-container>
  </section>
</template>

<style scoped>
#about {
  background-image: url("~@/assets/img/bgDownload.jpg");
  background-attachment: fixed;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  /* height: 500px; */
}

#about .container,
#about .row {
  /* height: 100%; */
}
/* #about {
  background-color: #f4f7f5;
} */
</style>
