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
            </v-row>

            <v-simple-table dark class="mt-7">
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
          period: "2021 Dec — Present",
          experience:
            "Full Stack Web Developer at WeClever.co (focused on Front-end). \
            Using Vue.js, TypeScript, Node.js, CSS, MySQL and AWS cloud services on a daily basis",
        },
        {
          period: "2019 Feb — 2021 Dec",
          experience: "Systems Analysis and Development, UNIP (University)",
        },
        {
          period: "2017 Mar — 2020 Dec",
          experience: "Administrative Assistant",
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
  overflow-x: hidden !important;
}
</style>
