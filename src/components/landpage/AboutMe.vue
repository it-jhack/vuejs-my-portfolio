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
                  My name is Thiago Amaral, I'm a brazilian
                  <span class="bold">Junior Full Stack Web Developer</span>
                  focused on Front-end. Most of what I know I learned by myself
                  online. I have a degree in System Analysis and Development and
                  also a previous Engineering degree.
                </p>
              </div>

              <v-expansion-panels dark multiple>
                <v-expansion-panel>
                  <v-expansion-panel-header class="skills-dropdown">
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
                      I started working as a Front-end developer in June 2021,
                      and as a Full Stack developer in December of the same
                      year.
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
                  <v-expansion-panel-header class="skills-dropdown">
                    Soft Skills
                  </v-expansion-panel-header>
                  <v-expansion-panel-content>
                    <div>
                      Soft skills can be fairly more valuable than hard skills
                      in the beginning of a career. It takes only a few months
                      to train a person to do complex tasks, but to change a
                      person's character and behavior can take a lifetime.
                    </div>
                    <div>
                      <div class="skill-bold mt-4">Proactivity</div>
                      <div class="mt-1 ml-4">
                        Getting the job done is not enough, getting it well done
                        is a must. This is an important skill in order to avoid
                        technical debt which can generate the awful feeling of
                        being always chasing one's own tail.
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
                        available online. It's essential for a developer to be
                        able to find similar solutions independently, and to
                        apply them to your context and project.
                      </div>
                    </div>
                    <div>
                      <div class="skill-bold mt-4">Friendliness</div>
                      <div class="mt-1 ml-4">
                        People consider me to be very friendly, even for
                        brazilian standards 😁
                      </div>
                    </div>
                  </v-expansion-panel-content>
                </v-expansion-panel>

                <v-expansion-panel>
                  <v-expansion-panel-header class="skills-dropdown">
                    Idioms
                  </v-expansion-panel-header>
                  <v-expansion-panel-content>
                    <div class="skills">
                      <p class="idiom-title">
                        <img
                          src="@/assets/img/brazil_icon.jpg"
                          max-height="40px"
                          max-width="30px"
                        />&nbsp; Brazilian Portuguese (Native)
                      </p>
                      <ul class="skill-ul">
                        <li class="skill-li">
                          <span class="skill-span pt-r"></span>
                          <p class="skill-text">
                            <span class="skill-bold">Reading:</span> Excellent
                          </p>
                        </li>
                        <li class="skill-li">
                          <span class="skill-span pt-w"></span>
                          <p class="skill-text">
                            <span class="skill-bold">Writing:</span>
                            Excellent
                          </p>
                        </li>
                        <li class="skill-li">
                          <span class="skill-span pt-l"></span>
                          <p class="skill-text">
                            <span class="skill-bold">Listening:</span>
                            Excellent
                          </p>
                        </li>
                        <li class="skill-li">
                          <span class="skill-span pt-s"></span>
                          <p class="skill-text">
                            <span class="skill-bold">Speaking:</span>
                            Excellent
                          </p>
                        </li>
                      </ul>

                      <p class="idiom-title">
                        <img
                          src="@/assets/img/us-icon.png"
                          max-height="40px"
                          max-width="30px"
                        />&nbsp; English (Fluent)
                      </p>
                      <ul class="skill-ul">
                        <li class="skill-li">
                          <span class="skill-span en-r"></span>
                          <p class="skill-text">
                            <span class="skill-bold">Reading:</span>
                            Fluent
                          </p>
                        </li>
                        <li class="skill-li">
                          <span class="skill-span en-w"></span>
                          <p class="skill-text">
                            <span class="skill-bold">Writing:</span>
                            Fluent
                          </p>
                        </li>
                        <li class="skill-li">
                          <span class="skill-span en-l"></span>
                          <p class="skill-text">
                            <span class="skill-bold">Listening:</span>
                            Fluent
                          </p>
                        </li>
                        <li class="skill-li">
                          <span class="skill-span en-s"></span>
                          <p class="skill-text">
                            <span class="skill-bold">Speaking:</span>
                            Fluent
                          </p>
                        </li>
                      </ul>

                      <p class="idiom-title">
                        <img
                          src="@/assets/img/spain_flag.png"
                          max-height="40px"
                          max-width="30px"
                        />&nbsp; Spanish (Good)
                      </p>
                      <ul class="skill-ul">
                        <li class="skill-li">
                          <span class="skill-span sp-r"></span>
                          <p class="skill-text">
                            <span class="skill-bold">Reading:</span>
                            Very Good
                          </p>
                        </li>
                        <li class="skill-li">
                          <span class="skill-span sp-w"></span>
                          <p class="skill-text">
                            <span class="skill-bold">Writing:</span>
                            Very Good
                          </p>
                        </li>
                        <li class="skill-li">
                          <span class="skill-span sp-l"></span>
                          <p class="skill-text">
                            <span class="skill-bold">Listening:</span>
                            Good
                          </p>
                        </li>
                        <li class="skill-li">
                          <span class="skill-span sp-s"></span>
                          <p class="skill-text">
                            <span class="skill-bold">Speaking:</span>
                            Communicable
                          </p>
                        </li>
                      </ul>
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
/* #about {
  background-size: cover;
  background-position: center;
} */

#about .container,
#about .row {
  height: 100%;
}

.desktop-bg {
  background-image: url("~@/assets/img/bgDownload.jpg");
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
  font-size: 22px;
}

.skills-dropdown {
  font-size: 16px;
}

/* Skill Bars */
.skills {
  width: 93%;
  position: relative;
  float: left;
  padding: 15px 0;
}
.skill-ul {
  padding-top: 30px;
}
.skill-li {
  margin-bottom: 50px;
  background: #dededed5;
  height: 6px;
  list-style-type: none;
}
.skill-text {
  font-style: italic;
  font-size: 18px;
  position: relative;
  top: -30px;
}
.skill-bold {
  font-weight: 600;
}
.skill-span {
  height: inherit;
  background-color: #009600da;
  /* background: linear-gradient(90deg, #009600da, #009600da); */
  background: #009600da;
  position: absolute;
}

.pt-r {
  width: 96.2%;
  animation: pt-r 1s ease-out;
}
.pt-w {
  width: 96.2%;
  animation: pt-w 1s ease-out;
}
.pt-l {
  width: 96.2%;
  animation: pt-l 1s ease-out;
}
.pt-s {
  width: 96.2%;
  animation: pt-s 1s ease-out;
}

.en-r {
  width: 93%;
  animation: en-r 1s ease-out;
}
.en-w {
  width: 93%;
  animation: en-w 1s ease-out;
}
.en-l {
  width: 93%;
  animation: en-l 1s ease-out;
}
.en-s {
  width: 93%;
  animation: en-s 1s ease-out;
}

.sp-r {
  width: 85%;
  animation: sp-r 1s ease-out;
}
.sp-w {
  width: 80%;
  animation: sp-w 1s ease-out;
}
.sp-l {
  width: 70%;
  animation: sp-l 1s ease-out;
}
.sp-s {
  width: 60%;
  animation: sp-s 1s ease-out;
}

/* idioms */
@keyframes pt-r {
  0% {
    width: 0px;
  }
  100% {
    width: 93%;
  }
}
@keyframes pt-w {
  0% {
    width: 0px;
  }
  100% {
    width: 93%;
  }
}
@keyframes pt-l {
  0% {
    width: 0px;
  }
  100% {
    width: 93%;
  }
}
@keyframes pt-s {
  0% {
    width: 0px;
  }
  100% {
    width: 93%;
  }
}

@keyframes en-r {
  0% {
    width: 0px;
  }
  100% {
    width: 90%;
  }
}
@keyframes en-w {
  0% {
    width: 0px;
  }
  100% {
    width: 90%;
  }
}
@keyframes en-l {
  0% {
    width: 0px;
  }
  100% {
    width: 90%;
  }
}
@keyframes en-s {
  0% {
    width: 0px;
  }
  100% {
    width: 90%;
  }
}

@keyframes sp-r {
  0% {
    width: 0px;
  }
  100% {
    width: 85%;
  }
}
@keyframes sp-w {
  0% {
    width: 0px;
  }
  100% {
    width: 80%;
  }
}
@keyframes sp-l {
  0% {
    width: 0px;
  }
  100% {
    width: 70%;
  }
}
@keyframes sp-s {
  0% {
    width: 0px;
  }
  100% {
    width: 60%;
  }
}
</style>
