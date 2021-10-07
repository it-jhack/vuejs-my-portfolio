<template>
  <section id="pricing">
    <!-- <v-parallax dark src="@/assets/img/bgHero.jpg" height="750">
      <v-row align="center" justify="center">
        <v-col cols="10">
          <v-row align="center" justify="center">
            <v-col cols="12" md="6" xl="8">
              <h1 class="display-2 font-weight-bold mb-4">
                Hi, my name is Thiago
              </h1>
              <h1 class="font-weight-light">
                I'm an avid self-taught student who likes to crush programming
                and networking topics on a daily basis.
              </h1>
              <v-btn
                rounded
                outlined
                large
                dark
                @click="$vuetify.goTo('#features')"
                class="mt-5"
              >
                Saiba mais
                <v-icon class="ml-2">mdi-arrow-down</v-icon>
              </v-btn>
            </v-col>
            <v-col cols="12" md="6" xl="4" class="hidden-sm-and-down"> </v-col>
          </v-row>
        </v-col>
      </v-row>
      <div class="svg-border-waves text-white">
        <v-img src="@/assets/img/borderWaves.svg" />
      </div>
    </v-parallax> -->
    <!-- <v-parallax height="500px" src="@/assets/img/big_data1.jpg"> -->

    <v-row align="top" justify="center">
      <v-col cols="10">
        <v-row align="top" justify="center">
          <v-col cols="12" md="6" xl="8">
            <br />
            <h1 class="display-1 mb-4 small-text-shadow">/cat my_trajectory</h1>
            <!-- <v-data-table
                :headers="headers"
                :items="experiences"
                hide-default-header="true"
                hide-default-footer="true"
                light="false"
                dark="true"
                item-key="name"
                class="elevation-1"
              ></v-data-table> -->
            <v-simple-table dark>
              <template v-slot:default>
                <!-- <thead>
                    <tr>
                      <th class="text-left">Name</th>
                      <th class="text-left">Calories</th>
                    </tr>
                  </thead> -->
                <tbody>
                  <tr v-for="item in experiences" :key="item.period">
                    <td>{{ item.period }}</td>
                    <td>{{ item.experience }}</td>
                  </tr>
                </tbody>
              </template>
            </v-simple-table>
          </v-col>
          <!-- <v-col cols="12" md="6" xl="4" class="hidden-sm-and-down"> </v-col> -->
        </v-row>
      </v-col>
    </v-row>
    <!-- #!DELETE? -->
    <!-- <div class="svg-border-waves text-white">
        <v-img src="@/assets/img/borderWaves.svg" />
      </div> -->

    <!-- </v-parallax> -->
  </section>
</template>

<script>
export default {
  data() {
    return {
      dialog: false,
      headers: [
        {
          text: " ",
          align: "start",
          value: "period",
        },
        { text: " ", value: "experience" },
      ],
      experiences: [
        {
          period: "2019 Feb — Present",
          experience: "Systems Analysis and Development student at UNIP",
        },
        {
          period: "2018 Dec — 2099",
          experience: "Self-taught IT student",
        },
        {
          period: "2017 Mar — 2020 Dec",
          experience: "Office Assistant",
        },
        {
          period: "2016 Sep — Dec",
          experience: "Intern at Duratex - Agudos, Brazil.",
        },
        {
          period: "2015 Apr — Jul",
          experience:
            "Business Intelligence Assistant intern at FPInnovations - Vancouver, Canada.",
        },
        {
          period: "2014 Sep — 2015 Apr",
          experience:
            "Internship Scholarship at University of British Columbia (UBC) - Vancouver, Canada",
        },

        {
          period: "2011 — 2016",
          experience:
            "Engineering, Forestry. Bachelor degree at UNESP - Sao Paulo State University.",
        },
      ],
    };
  },
  watch: {
    dialog(value) {
      if (!value) {
        this.pause();
      }
    },
  },
  // #!DELETE
  // methods: {
  //   ready(event) {
  //     this.player = event.target;
  //   },
  //   playing(event) {
  //     // The player is playing a video.
  //   },
  //   change() {
  //     // when you change the value, the player will also change.
  //     // If you would like to change `playerVars`, please change it before you change `videoId`.
  //     // If `playerVars.autoplay` is 1, `loadVideoById` will be called.
  //     // If `playerVars.autoplay` is 0, `cueVideoById` will be called.
  //     this.videoId = "another video id";
  //   },
  //   stop() {
  //     this.player.stopVideo();
  //   },
  //   pause() {
  //     this.player.pauseVideo();
  //   },
  // },
};
</script>

<style>
.btn-play {
  transition: 0.2s;
}

.svg-border-waves .v-image {
  position: absolute;
  bottom: 0;
  left: 0;
  height: 3rem;
  width: 100%;
  overflow: hidden;
}

#pricing {
  height: 500px;
  width: 100%;
  background-color: rgb(41, 41, 41);
}

.svg-border-waves img {
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  margin-bottom: -2px;
  z-index: -1;
}

.card {
  min-height: 500px;
  padding: 10px;
  transition: 0.5s ease-out;
}

.card .v-image {
  margin-bottom: 15px;
  transition: 0.75s;
}

.card h1 {
  margin-bottom: 10px;
}

.zoom-efect {
  transform: scale(1.1);
}

.up {
  transform: translateY(-20px);
  transition: 0.5s ease-out;
}

section {
  position: relative;
}

#parallax {
  background-attachment: fixed;
  background-size: 100% auto;
  height: 900px;
}
</style>
