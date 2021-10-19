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
              <h1 class="font-weight-light justified">
                My name is Thiago Amaral, I'm a web developer and a
                <b>Systems Analysis and Development</b>
                student from Brazil, although most of what I know I learned by
                myself online. I also have a previous Engineering degree.
              </h1>
              <br />

              <v-expansion-panels dark multiple>
                <v-expansion-panel>
                  <v-expansion-panel-header>
                    Hard Skills
                  </v-expansion-panel-header>
                  <v-expansion-panel-content>
                    <div class="skills">
                      <h2>Front-End</h2>
                      <ul>
                        <li><span class="html5"></span><em>HTML</em></li>
                        <li><span class="css3"></span><em>CSS</em></li>
                        <li><span class="js"></span><em>Javascript</em></li>
                        <li><span class="jquery"></span><em>jQuery</em></li>
                      </ul>
                      <h2>Frameworks</h2>
                      <ul>
                        <li>
                          <span class="wordpress"></span><em>Wordpress</em>
                        </li>
                        <li><span class="magento"></span><em>Magento</em></li>
                      </ul>
                      <h2>Applications</h2>
                      <ul>
                        <li>
                          <span class="photoshop"></span
                          ><em>Adobe Photoshop</em>
                        </li>
                        <li>
                          <span class="illustrator"></span
                          ><em>Adobe Illustrator</em>
                        </li>
                      </ul>
                    </div>
                  </v-expansion-panel-content>
                </v-expansion-panel>

                <v-expansion-panel>
                  <v-expansion-panel-header>
                    Soft Skills
                  </v-expansion-panel-header>
                  <v-expansion-panel-content>
                    <p>
                      I consider soft skills to be far more valuable than hard
                      skills for a person at the beginning of a career. It takes
                      only a few months to train a person to do complex tasks at
                      a fairly good pace. But to change a person's character and
                      behavior... that can take a lifetime!
                    </p>

                    <p>
                      <b>PROACTIVE:</b> I always try to deliver a little extra
                      from what is required
                    </p>
                    <p>
                      <b>TIME MANAGER:</b> Time is amongst the top most
                      important resources. I constantly measure and evaluate how
                      I spend my time
                    </p>
                    <p>
                      <b>FRIENDLY:</b> People consider me a friendly person. A
                      toxic person can demotivate a whole team
                    </p>
                    <p>
                      <b>QUICK LEARNER:</b> As much as stating this can be very
                      cliché, I've actually been complimented by been able to
                      quickly adapt to tools and languages I've never used
                      before
                    </p>
                    <p>
                      <b>SELF-TAUGHT:</b> Nowadays with the vast incredible
                      content available online, it's crucial to be able to find
                      solutions independently, without overwhelming colleagues
                      as a crutch for every single doubt
                    </p>
                  </v-expansion-panel-content>
                </v-expansion-panel>

                <v-expansion-panel>
                  <v-expansion-panel-header> Idioms </v-expansion-panel-header>
                  <v-expansion-panel-content>
                    <div class="skills">
                      <h2>
                        <img
                          src="@/assets/img/brazil_icon.jpg"
                          max-height="40px"
                          max-width="30px"
                        />&nbsp; Brazilian Portuguese (Native)
                      </h2>
                      <ul>
                        <li>
                          <span class="pt-r"></span
                          ><em><b>Reading:</b> Excellent</em>
                        </li>
                        <li>
                          <span class="pt-w"></span
                          ><em><b>Writing:</b> Excellent</em>
                        </li>
                        <li>
                          <span class="pt-l"></span
                          ><em><b>Listening:</b> Excellent</em>
                        </li>
                        <li>
                          <span class="pt-s"></span
                          ><em><b>Speaking:</b> Excellent</em>
                        </li>
                      </ul>

                      <h2>
                        <img
                          src="@/assets/img/us-icon.png"
                          max-height="40px"
                          max-width="30px"
                        />&nbsp; English (Fluent)
                      </h2>
                      <ul>
                        <li>
                          <span class="en-r"></span
                          ><em><b>Reading:</b> Fluent</em>
                        </li>
                        <li>
                          <span class="en-w"></span
                          ><em><b>Writing:</b> Fluent</em>
                        </li>
                        <li>
                          <span class="en-l"></span
                          ><em><b>Listening:</b> Fluent</em>
                        </li>
                        <li>
                          <span class="en-s"></span
                          ><em><b>Speaking:</b> Fluent</em>
                        </li>
                      </ul>

                      <h2>
                        <img
                          src="@/assets/img/spain_flag.png"
                          max-height="40px"
                          max-width="30px"
                        />&nbsp; Spanish (Good)
                      </h2>
                      <ul>
                        <li>
                          <span class="sp-r"></span
                          ><em><b>Reading:</b> Very Good</em>
                        </li>
                        <li>
                          <span class="sp-w"></span
                          ><em><b>Writing:</b> Very Good</em>
                        </li>
                        <li>
                          <span class="sp-l"></span
                          ><em><b>Listening:</b> Good</em>
                        </li>
                        <li>
                          <span class="sp-s"></span
                          ><em><b>Speaking:</b> Communicable</em>
                        </li>
                      </ul>
                    </div>
                  </v-expansion-panel-content>
                </v-expansion-panel>
                <v-expansion-panel>
                  <v-expansion-panel-header> Hobbies </v-expansion-panel-header>
                  <v-expansion-panel-content>
                    Some of my hobbies are working out, watching good movies and
                    I absolutely love to improve my coding skills by building
                    small projects and dismantling open-source code to see how
                    it works :)
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

.justified {
  text-align: justify;
  text-justify: inter-word;
}

@import url("https://fonts.googleapis.com/css?family=Open+Sans+Condensed:300,300i,700");

html {
  background: #f4f4f4;
}

body {
  font-family: "Open Sans Condensed", sans-serif;
  font-size: 12px;
  color: #444;
  width: 360px;
  margin: 20px auto;
  background-color: pink;
}

h2 {
  font-size: 24px;
  margin-bottom: 25px;
  font-weight: 700;
}

/* Skill Bars */

.skills {
  width: 90%;
  position: relative;
  float: left;
  padding: 30px 0;
}

ul {
  padding-top: 30px;
}
li {
  margin-bottom: 50px;
  background: #dededed5;
  height: 6px;
  list-style-type: none;
}
em {
  font-size: 18px;
  position: relative;
  top: -30px;
}
span {
  height: inherit;
  background-color: #009600da;
  background: linear-gradient(90deg, #009600da, #009600da);
  position: absolute;
}

.html5 {
  width: 90%;
  animation: html5 1s ease-out;
}
.css3 {
  width: 80%;
  animation: css3 1s ease-out;
}
.js {
  width: 50%;
  animation: js 1s ease-out;
}
.jquery {
  width: 60%;
  animation: jquery 1s ease-out;
}
.wordpress {
  width: 50%;
  animation: wordpress 1s ease-out;
}
.magento {
  width: 60%;
  animation: magento 1s ease-out;
}
.photoshop {
  width: 90%;
  animation: photoshop 1s ease-out;
}
.illustrator {
  width: 80%;
  animation: illustrator 1s ease-out;
}

.pt-r {
  width: 93%;
  animation: pt-r 1s ease-out;
}
.pt-w {
  width: 93%;
  animation: pt-w 1s ease-out;
}
.pt-l {
  width: 93%;
  animation: pt-l 1s ease-out;
}
.pt-s {
  width: 93%;
  animation: pt-s 1s ease-out;
}

.en-r {
  width: 90%;
  animation: en-r 1s ease-out;
}
.en-w {
  width: 90%;
  animation: en-w 1s ease-out;
}
.en-l {
  width: 90%;
  animation: en-l 1s ease-out;
}
.en-s {
  width: 90%;
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

@keyframes html5 {
  0% {
    width: 0px;
  }
  100% {
    width: 90%;
  }
}
@keyframes css3 {
  0% {
    width: 0px;
  }
  100% {
    width: 80%;
  }
}
@keyframes js {
  0% {
    width: 0px;
  }
  100% {
    width: 50%;
  }
}
@keyframes jquery {
  0% {
    width: 0px;
  }
  100% {
    width: 60%;
  }
}
@keyframes wordpress {
  0% {
    width: 0px;
  }
  100% {
    width: 50%;
  }
}
@keyframes magento {
  0% {
    width: 0px;
  }
  100% {
    width: 60%;
  }
}
@keyframes photoshop {
  0% {
    width: 0px;
  }
  100% {
    width: 90%;
  }
}
@keyframes illustrator {
  0% {
    width: 0px;
  }
  100% {
    width: 80%;
  }
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
