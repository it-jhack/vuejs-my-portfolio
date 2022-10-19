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
                    <p>
                      Here are some examples of technologies that I have already
                      worked with:
                    </p>
                    <ul class="mb-4">
                      <li>Vue.js</li>
                      <li>TypeScript (mostly) and JavaScript</li>
                      <li>JSON, Rest APIs, CORS</li>
                      <li>CSS and SCSS</li>
                      <li>Flexbox and Grid system</li>
                      <li>BootStrap Vue</li>
                      <li>Node.js (also in TypeScript)</li>
                      <li>MySQL and NoSQL</li>
                      <li>AWS Cloud Services</li>
                      <li>Google Tag Manager</li>
                      <li>jQuery</li>
                      <li>GitFlow, Agile and Scrum methodologies</li>
                    </ul>
                    <p>
                      I started working as an intern in Front-end development in
                      June 2021, and was effectively hired in December of the
                      same year.
                    </p>
                    <p>
                      Although I work focused mainly on front-end, I have worked
                      in backend features and hotfixes on numerous occasions,
                      which gave me an overall good understanding of APIs, how
                      to better structure the front-end, and how to effectively
                      connect it to the back-end.
                    </p>
                    <p>
                      One year of experience might not look like much, but I
                      feel that I've learned the equivalent of so much more
                      during this time. Time flies by when I code because I
                      absolutely love it. I guess that's the secret to learn
                      quickly in little time :D
                    </p>
                    <p>
                      I also have experimented with
                      <span class="bold">Bug Hunting</span>
                      in the past, which gave me a good general understanding of
                      web vulnerabilities. As described in the Projects section
                      of this page, during this period I developed a tool in
                      Python that can identify Subdomain Takeover
                      vulnerabilities.
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
                      at the beginning of a career. It takes only a few months
                      to train a person to do complex tasks, but to change a
                      person's character and behavior can take a lifetime.
                    </div>
                    <div>
                      <div class="skill-bold mt-4">Proactivity</div>
                      <div class="mt-1 ml-4">
                        I try to proactively plan before execution. Getting all
                        jobs done in any way as fast as possible is a trap that
                        will quickly build up technical debt. On the other hand,
                        planning too much can be even worse. Balance between
                        proactive planning and execution is key.
                      </div>
                    </div>
                    <div>
                      <div class="skill-bold mt-4">Time Management</div>
                      <div class="mt-1 ml-4">
                        Time is the most valuable resource there is. There is
                        only a finite amount and we don't even know for sure how
                        much of it we got left. I constantly measure and
                        evaluate how I spend my time, seeking what can bring me
                        the best cost-benefit in the long run.
                      </div>
                    </div>
                    <div>
                      <div class="skill-bold mt-4">Quick Learning</div>
                      <div class="mt-1 ml-4">
                        I know that stating this can be very cliché, but I've
                        actually been complimented for being able to quickly
                        adapt to tools and languages I've never used before.
                      </div>
                    </div>
                    <div>
                      <div class="skill-bold mt-4">Self-taught</div>
                      <div class="mt-1 ml-4">
                        There is a vast magnitude of incredible content
                        available online. A developer should be able to find
                        similar solutions independently, and apply them to
                        context of the project.
                      </div>
                    </div>
                    <div>
                      <div class="skill-bold mt-4">Friendliness</div>
                      <div class="mt-1 ml-4">
                        People consider me to be very friendly, even for
                        Brazilian standards 😁
                      </div>
                    </div>
                  </v-expansion-panel-content>
                </v-expansion-panel>

                <v-expansion-panel>
                  <v-expansion-panel-header>
                    Idioms
                  </v-expansion-panel-header>
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
                        <span class="ml-2">
                          English (Fluent)
                        </span>
                      </p>

                      <p class="idiom-title">
                        <img
                          src="@/assets/img/spain_flag.png"
                          class="idiom-flag"
                        />
                        <span class="ml-2">
                          Spanish (Communicable)
                        </span>
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
  transform: translate(0, 4px)
}
</style>
