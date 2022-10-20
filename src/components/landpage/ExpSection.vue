<template>
  <section class="pb-8" id="experience" height="100%">
    <v-row justify="center" height="100%">
      <v-col cols="10">
        <v-row justify="center">
          <v-col cols="12" md="7" xl="9">
            <div class="terminal-title mt-5 mb-4">/cat my_journey</div>

            <v-row class="d-flex justify-content-space-evenly mt-6 mb-4">
              <v-btn
                rounded
                outlined
                href="https://www.linkedin.com/in/thiago-de-paula-amaral/"
                target="_blank"
                large
                color="white"
                class="mt-4"
              >
                <v-icon class="mr-2"> mdi-linkedin </v-icon>
                <span>Check my Linkedin</span>
              </v-btn>
            </v-row>

            <v-simple-table dark class="mt-7">
              <template v-slot:default>
                <tbody>
                  <tr v-for="item in experiences" :key="item.period">
                    <td class="pt-2 pb-2">
                      <img v-if="item.image" :src="item.image" class="logo" />
                      <span class="period">{{ item.period }}</span>
                    </td>
                    <td class="pt-2 pb-2">
                      {{ item.experience }}
                    </td>
                  </tr>
                </tbody>
              </template>
            </v-simple-table>
          </v-col>
        </v-row>
      </v-col>
    </v-row>
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
          image: "logo-weclever.png",
          period: "2021 Dec — Present",
          experience:
            "Front-end Web Developer at WeClever.co, a fast-paced,\
            quick-evolving B2B Brazilian startup. Sometimes I also \
            work in the Back-end. Here I enhanced my skills in \
            Vue.js, TypeScript, Node.js, CSS, MySQL \
            and AWS cloud services.",
        },
        {
          image: "logo-flowdev.png",
          period: "2021 Jun — 2021 Dec",
          experience:
            "Front-end Developer Intern at FlowDev Systems, a company that \
            develops small custom commercial web systems. While working here, I \
            developed my skills using Vue.js, JavaScript, CSS, Vuetify, and \
            calling APIs using Axios and",
        },
        {
          image: "logo-unip.png",
          period: "2019 — 2021",
          experience: "Systems Analysis and Development, UNIP (University)",
        },
        {
          image: "logo-a&a.png",
          period: "2017 — 2020",
          experience: "Administrative Assistant, A&A Furnitures Ltd.",
        },
        {
          image: "logo-fpi.png",
          period: "2015",
          experience:
            "Business Intelligence Assistant intern at FPInnovations - Vancouver, Canada.",
        },
        {
          image: "logo-ubc.png",
          period: "2014 — 2015",
          experience:
            "Internship Scholarship at University of British Columbia (UBC) - Vancouver, Canada",
        },
        {
          image: "logo-unesp.png",
          period: "2011 — 2016",
          experience:
            "Engineering, Forestry. Bachelor's degree at UNESP - Sao Paulo State University.",
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
};
</script>

<style scoped>
#experience {
  width: 100%;
  background-color: #292929;
  overflow-x: hidden !important;
}

.logo {
  display: grid;
  justify-content: center;
  margin: 10px 0;
  max-width: 80px;
  max-height: 35px;
}

.period {
  color: #c4c4c4;
}
</style>
