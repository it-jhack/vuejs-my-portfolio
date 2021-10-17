<template>
  <section id="about">
    <v-container fluid>
      <v-row align="center" justify="center">
        <v-col cols="10">
          <v-row justify="center">
            <v-col sm="4" class="hidden-xs-only">
              <v-img
                src="@/assets/img/thiago.jpg"
                class="d-block ml-auto mr-auto rounded-corners"
                max-width="200px"
              />
            </v-col>
            <v-col cols="12" sm="8" class="white--text text-left">
              <h1 class="font-weight-light display-2 mb-2">/whoami</h1>
              <h1 class="font-weight-light">
                My name is Thiago Amaral, I'm a web developer and a
                <b>Systems Analysis and Development</b>
                student from Brazil, although most of what I know I learned by
                myself online. I also have a previous Engineering degree.
              </h1>
              <br />
              <h1 class="font-weight-light">
                I love to code and to learn by building small projects. Some of
                my hobbies are working out, watching movies and dismantling
                softwares and hardwares to see how they work. I rarely have been
                gaming for the past few years but I also enjoy it :)
              </h1>
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
  /* height: 750px; */
}

#about .container,
#about .row {
  height: 100%;
}

.rounded-corners {
  border-radius: 20%;
}
</style>
