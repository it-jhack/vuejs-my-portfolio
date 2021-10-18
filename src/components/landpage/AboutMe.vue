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
                    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed
                    do eiusmod tempor incididunt ut labore et dolore magna
                    aliqua. Ut enim ad minim veniam, quis nostrud exercitation
                    ullamco laboris nisi ut aliquip ex ea commodo consequat.
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
                        <li><span class="html5"></span><em>Reading</em></li>
                        <li><span class="css3"></span><em>Writing</em></li>
                        <li><span class="js"></span><em>Listening</em></li>
                        <li><span class="jquery"></span><em>Speaking</em></li>
                      </ul>

                      <h2>
                        <img
                          src="@/assets/img/us-icon.png"
                          max-height="40px"
                          max-width="30px"
                        />&nbsp; English
                      </h2>
                      <ul>
                        <li><span class="html5"></span><em>Reading</em></li>
                        <li><span class="css3"></span><em>Writing</em></li>
                        <li><span class="js"></span><em>Listening</em></li>
                        <li><span class="jquery"></span><em>Speaking</em></li>
                      </ul>

                      <h2>
                        <img
                          src="@/assets/img/spain_flag.png"
                          max-height="40px"
                          max-width="30px"
                        />&nbsp; Spanish
                      </h2>
                      <ul>
                        <li><span class="html5"></span><em>Reading</em></li>
                        <li><span class="css3"></span><em>Writing</em></li>
                        <li><span class="js"></span><em>Listening</em></li>
                        <li><span class="jquery"></span><em>Speaking</em></li>
                      </ul>
                    </div>
                  </v-expansion-panel-content>
                </v-expansion-panel>
              </v-expansion-panels>

              <br />

              <h1 class="font-weight-light justified">
                I love to improve my coding skills by building small projects.
                Some of my hobbies are working out, watching good movies and
                dismantling softwares and hardwares to see how they work :)
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

/* .skills {
  width: inherit;
  position: relative;
  float: left;
  padding: 30px 0;
  ul {
    padding-top: 30px;
    & > li {
      margin-bottom: 50px;
      background: #dedede;
      height: 6px;
      & em {
        font-size: 18px;
        position: relative;
        top: -30px;
      }
      & span {
        height: inherit;
        background-color: #94c245;
        background: linear-gradient(90deg, #76b82a, #aecd60);
        position: absolute;
      }
    }
  } */

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
  background: #dededea1;
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
  background-color: #94c245;
  background: linear-gradient(90deg, #94c245, #94c245);
  position: absolute;
}

.html5 {
  width: 90%;
  animation: html5 2s ease-out;
}
.css3 {
  width: 80%;
  animation: css3 2s ease-out;
}
.js {
  width: 50%;
  animation: js 2s ease-out;
}
.jquery {
  width: 60%;
  animation: jquery 2s ease-out;
}
.wordpress {
  width: 50%;
  animation: wordpress 2s ease-out;
}
.magento {
  width: 60%;
  animation: magento 2s ease-out;
}
.photoshop {
  width: 90%;
  animation: photoshop 2s ease-out;
}
.illustrator {
  width: 80%;
  animation: illustrator 2s ease-out;
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
</style>
