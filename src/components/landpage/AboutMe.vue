<template>
  <section
    id="about"
    :class="$store.state.isMobile ? 'mobile-bg' : 'desktop-bg'"
  >
    <v-container fluid>
      <v-row align="center" justify="center">
        <v-col cols="10">
          <v-row justify="center">
            <v-col sm="4">
              <v-img
                src="@/assets/img/thiago.jpg"
                class="d-block ml-auto mr-auto mt-4 rounded-corners"
                max-width="200px"
              />
            </v-col>
            <v-col cols="12" sm="8" class="white-color">
              <div>
                <p class="terminal-title mb-2 mt-4">/whoami</p>
                <p
                  class="p-text mt-5"
                  :class="$store.state.isMobile ? '' : 'justified'"
                >
                  My name is Thiago Amaral, I'm a Brazilian
                  <span class="bold">Front-end Developer</span>, but sometimes I
                  morph into Full Stack mode 😄. I've been studying programming
                  on my own since 2018 and have been working professionally on
                  front-end development since mid-2021. I have a degree in
                  Systems Analysis and Development and also a previous
                  Engineering degree.
                </p>
              </div>

              <v-expansion-panels dark multiple>
                <v-expansion-panel>
                  <v-expansion-panel-header>
                    Hard Skills
                  </v-expansion-panel-header>
                  <v-expansion-panel-content>
                    <ul class="mb-4">
                      <li>
                        Vue.js, Vuex, Nuxt.js, Vue Router (also some React)
                      </li>
                      <li>TypeScript and JavaScript</li>
                      <li>Cypress (automated tests)</li>
                      <li>JSON, Rest APIs, CORS</li>
                      <li>Css and Sass/scss</li>
                      <li>Flexbox and Grid system</li>
                      <li>BootStrap Vue</li>
                      <li>Node.js (also in TypeScript)</li>
                      <li>MySQL and NoSQL</li>
                      <li>AWS Cloud Services</li>
                      <li>Google Tag Manager</li>
                      <li>GitFlow, Agile and Scrum methodologies</li>
                    </ul>
                    <p>
                      I started working on front-end web development as an
                      intern in June 2021 and was hired in December 2021; I’ve
                      been studying programming and IT independently since 2018.
                    </p>
                    <p>
                      Front-end experience using Vue.js, TypeScript/JavaScript,
                      Cypress E2E automated testing, Sass/Scss, and Tailwindcss.
                    </p>
                    <p>
                      Back-end experience with Node.js, Express.js, and
                      Insomnia/Postman.
                    </p>
                    <p>
                      Some Database experience with SQL (AWS RDS) and NoSQL
                      technologies (AWS DynamoDB), using DataGrip and MySQL
                      Workbench as SQL IDE.
                    </p>
                    <p>
                      I love to use Linux Debian OS and Bash/Unix Shell
                      scripting to optimize tasks.
                    </p>
                    <p>
                      Good knowledge of networks and common cyber-security
                      threats.
                    </p>
                    <p>
                      Here are some examples of technologies that I have already
                      worked with:
                    </p>
                  </v-expansion-panel-content>
                </v-expansion-panel>

                <v-expansion-panel>
                  <v-expansion-panel-header>
                    Soft Skills
                  </v-expansion-panel-header>
                  <v-expansion-panel-content>
                    <div>
                      Soft skills can be fairly more valuable than hard skills
                      at the beginning of a career. Many complex hard skills can
                      be acquired within less than a few months, but to change a
                      person's character and behavior can take a lifetime.
                    </div>
                    <div>
                      <div class="skill-bold mt-4">🏃‍♂️ Proactivity</div>
                      <div class="mt-1 ml-4">
                        I try to proactively plan before execution. Getting all
                        jobs done in any way as fast as possible is a trap that
                        will quickly build up technical debt. On the other hand,
                        planning too much can be even worse. Balance between
                        proactive planning and execution is key.
                      </div>
                    </div>
                    <div>
                      <div class="skill-bold mt-4">🕒 Time Management</div>
                      <div class="mt-1 ml-4">
                        Time is the most valuable resource there is. There is
                        only a finite amount and we don't even know for sure how
                        much of it we got left. I constantly measure and
                        evaluate how I spend my time, seeking what can bring me
                        the best cost-benefit in the long run.
                      </div>
                    </div>
                    <div>
                      <div class="skill-bold mt-4">🧠 Quick Learning</div>
                      <div class="mt-1 ml-4">
                        I know that stating this can be very cliché, but I've
                        actually been complimented for being able to quickly
                        adapt to tools and languages I've never used before.
                      </div>
                    </div>
                    <div>
                      <div class="skill-bold mt-4">📚 Self-taught</div>
                      <div class="mt-1 ml-4">
                        There is a vast magnitude of incredible content
                        available online. A developer should be able to find
                        similar solutions independently, and apply them to
                        context of the project.
                      </div>
                    </div>
                    <div>
                      <div class="skill-bold mt-4">😁 Friendliness</div>
                      <div class="mt-1 ml-4">
                        People consider me to be very friendly.
                      </div>
                    </div>
                  </v-expansion-panel-content>
                </v-expansion-panel>

                <v-expansion-panel>
                  <v-expansion-panel-header> Idioms </v-expansion-panel-header>
                  <v-expansion-panel-content>
                    <div>
                      <p class="idiom-title">
                        <img
                          src="@/assets/img/brazil_icon.jpg"
                          class="idiom-flag"
                        />
                        <span class="ml-2">
                          Brazilian Portuguese (Native)
                        </span>
                      </p>

                      <p class="idiom-title">
                        <img
                          src="@/assets/img/us-icon.png"
                          class="idiom-flag"
                        />
                        <span class="ml-2"> English (Fluent) </span>
                      </p>

                      <p class="idiom-title">
                        <img
                          src="@/assets/img/spain_flag.png"
                          class="idiom-flag"
                        />
                        <span class="ml-2"> Spanish (Communicable) </span>
                      </p>
                    </div>
                  </v-expansion-panel-content>
                </v-expansion-panel>
              </v-expansion-panels>
            </v-col>
          </v-row>
        </v-col>
      </v-row>
    </v-container>
  </section>
</template>

<style scoped>
#about .container,
#about .row {
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
}

.rounded-corners {
  border-radius: 20%;
}

.justified {
  text-align: justify;
  text-justify: inter-word;
}

html {
  background: #f4f4f4;
}

.idiom-title {
  font-size: 16px;
}

.idiom-flag {
  max-height: 40px;
  max-width: 30px;
  transform: translate(0, 4px);
}
</style>
