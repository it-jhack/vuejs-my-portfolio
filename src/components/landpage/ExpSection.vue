<template>
  <section class="pb-8" id="experience" height="100%">
    <v-row align="top" justify="center" height="100%">
      <v-col cols="10">
        <v-row align="top" justify="center">
          <v-col cols="12" md="7" xl="9">
            <br />
            <h1 class="display-1 mb-4 small-text-shadow">/cat my_roadmap</h1>

            <v-btn
              rounded
              outlined
              href="https://drive.google.com/file/d/1WJerXKFDnReh05pwwSD2H2bXYeGxZkzQ/view?usp=sharing"
              target="_blank"
              large
              color="white"
              class="mt-4"
            >
              <v-icon class="mr-2"> mdi-download </v-icon>
              Curriculum Vitae &nbsp;
              <v-img src="@/assets/img/brazil_icon.jpg" />
            </v-btn>

            <br /><br />

            <v-simple-table dark>
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
  background-color: rgb(41, 41, 41);
}

h1 {
  color: white;
}
</style>
