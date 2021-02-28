<template>
  <div class="profile">
    <div class="container">
      <div class="row">
        <div class="col">
          <div class="profile__logo profile__header">shivam k.</div>
        </div>
        <div class="col">
          <ButtonGroup class="about_socialMedia">
            <Button icon="logo-linkedin"></Button>
            <Button icon="logo-twitter"></Button>
            <Button icon="ios-mail"></Button>
          </ButtonGroup>
        </div>
      </div>
      <div class="row hello__element">
        <div class="col-6 col-md-4">
          <div class="about_imagediv">
            <img class="about__image" src="../assets/aboutImage.jpg" />
          </div>
        </div>
        <div class="col-md-8">
          <div class="row hello__element">
            <div class="col">
              <div>
                <span class="hello__text">Hi, I'm Shivam</span>
                <Icon class="info__hi" type="ios-hand" />
              </div>
            </div>
          </div>
          <div class="row">
            <div class="col">
              <div>
                <span class="hello__text">Full Stack Developer</span>
                <!-- <span class="helloText">{{experienceText}}</span> -->
              </div>
            </div>
          </div>
          <div class="row">
            <div class="col">
              <div>
                <span class="about__text"
                  >A bagpacker, an explorer and Javascript enthusiast who loves
                  breaking down complex problems.</span
                >
                <div class="row about_buttons">
                  <div class="col-sm about_referenceButton">
                    <Button class="navButtons" type="primary" shape="circle"
                      >Projects</Button
                    >
                  </div>
                  <div class="col-sm about_referenceButton">
                    <Button class="navButtons" type="primary" shape="circle"
                      >Blogs</Button
                    >
                  </div>
                  <div class="col-sm about_referenceButton">
                    <Button class="navButtons" type="primary" shape="circle"
                      >Experience</Button
                    >
                  </div>
                </div>
                <!-- <span class="helloText">{{experienceText}}</span> -->
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import { Button, ButtonGroup } from "view-design";
export default {
  name: "Profile",
  components: {
    Button,
    ButtonGroup
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Caveat&family=Gloria+Hallelujah&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Caveat&family=Gloria+Hallelujah&family=Poppins&display=swap");
.profile {
  height: 100vh;
}
.profile__header {
  padding-top: 5px;
  font-family: Caveat;
  font-style: normal;
  font-weight: normal;
  color: #ffffff;
}
.profile__logo {
  font-size: 4vmax;
}
.hello__element {
  padding-top: 40px;
  text-align: center;
}
.hello__text {
  font-family: Poppins;
  font-style: normal;
  font-weight: bold;
  font-size: 4vmax;
  color: #ffffff;
  border: 1px solid #000000;
  text-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
}
.hello__dot {
  font-size: 26px;
  color: #32c766;
}
.about__text {
  font-family: Poppins;
  font-style: normal;
  font-weight: normal;
  font-size: 2vmax;
  color: #afabab;
}
.about__image {
  align-content: center;
  width: 20vmax;
  height: 20vmax;
}
.about_imagediv {
  padding-left: 15vh;
}
.about_referenceButton {
  padding: 2vh;
}
.about_buttons {
  padding-top: 8vh;
}
.info__hi {
  color: #ffd04d;
  font-size: 4vmax;
  animation-name: hi-animation; /* Refers to the name of your @keyframes element below */
  animation-duration: 2.5s; /* Change to speed up or slow down */
  animation-iteration-count: infinite; /* Never stop waving :) */
  transform-origin: 70% 70%; /* Pivot around the bottom-left palm */
  display: inline-block;
}
.navButtons {
  width: 30vh;
}
.about_socialMedia {
  float: right;
  padding: 5px;
}
@keyframes hi-animation {
  0% {
    transform: rotate(0deg);
  }
  10% {
    transform: rotate(14deg);
  } /* The following five values can be played with to make the waving more or less extreme */
  20% {
    transform: rotate(-8deg);
  }
  30% {
    transform: rotate(14deg);
  }
  40% {
    transform: rotate(-4deg);
  }
  50% {
    transform: rotate(10deg);
  }
  60% {
    transform: rotate(0deg);
  } /* Reset for the last half to pause */
  100% {
    transform: rotate(0deg);
  }
}
</style>
