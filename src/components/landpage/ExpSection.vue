<template>
  <section class="pb-8" id="experience" height="100%">
    <v-row align="top" justify="center" height="100%">
      <v-col cols="10">
        <v-row align="top" justify="center">
          <v-col cols="12" md="7" xl="9">
            <h1 class="display-1 mb-4 small-text-shadow">/cat my_roadmap</h1>

            <div class="d-flex justify-content-space-evenly">
              <v-btn
                rounded
                outlined
                href="https://drive.google.com/file/d/1BH-3ObjuuO5fkv09Rv5ixuop7oLxaoKJ/view?usp=sharing"
                target="_blank"
                large
                color="white"
                class="mt-4"
              >
                <v-icon class="mr-2"> mdi-download </v-icon>
                <span>Download Resume</span>
              </v-btn>

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
            </div>

            <v-simple-table dark class="mt-5">
              <template v-slot:default>
                <tbody>
                  <tr v-for="item in experiences" :key="item.period">
                    <td>{{ item.period }}</td>
                    <td>{{ item.experience }}</td>
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
          period: "Present Moment",
          experience: "Front-end developer, also improving my Back-end skills",
        },
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
};
</script>

<style scoped>
#experience {
  width: 100%;
  background-color: #292929;
}

h1 {
  color: white;
}
</style>
