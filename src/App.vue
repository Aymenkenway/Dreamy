<template>
  <v-app class="bg-black">
    <div class="v-main">
      <div class="Header"><Header /></div>
      <div class="vector1">
        <img src="./assets/icons/Vector1.png" alt="" />
      </div>
      <div class="hero">
        <img class="sub-hero1" src="./assets/icons/hero.png" alt="" />
        <div class="sub-hero2">
          <p class="we-help-you-to-grow">
            <span class="text-wrapper" style="font-weight: bold"
              >We Help you</span
            >
            <br />
            <span class="span">to grow your<br />Business</span>
          </p>
          <p class="sub-hero3">
            Lorem Ipsum has been the industry&#39;s standard dummy text ever
            since the 1500s, when an unknown printer took a galley of type and
            scrambled it to make a type specimen book.
          </p>

          <div class="sub-hero4"><div class="rectangle">GET STARTED</div></div>
        </div>
      </div>
    </div>
    <Swiper class="first-swiper" />
    <div class="hero2">
      <img class="sub2-hero1" src="./assets/icons/hero2.png" alt="" />
      <div class="sub2-hero2">
        <p class="we-help-you-to-grow">
          <span class="text-wrapper" style="font-weight: bold">About Us</span>
          <br />
          <span class="span">Fake or Real</span>
        </p>
        <p class="sub2-hero3">
          Lorem Ipsum has been the industry&#39;s standard dummy text ever since
          the 1500s, when an unknown printer took a galley of type and scrambled
          it to make a type specimen book.
        </p>
        <p class="sub2-hero3">
          Lorem Ipsum has been the industry&#39;s standard dummy text ever since
          the 1500s, when an unknown printer took a galley of type and scrambled
          it to make a type specimen book.
        </p>
        <div class="sub2-hero4"><div class="rectangle">EXPLORE MORE</div></div>
      </div>
    </div>
    <SwiperBottom class="second-swiper" />
    <Quotes />
    <div>
      <Footer />
    </div>
  </v-app>
</template>

<script>
import Home from './views/home/Home'
import Header from './components/Header'
import Swiper from './components/Swiper'
import SwiperBottom from './components/SwiperBottom'
import Quotes from './components/Quotes'
import Footer from './components/Footer.vue'
export default {
  name: 'App',

  components: {
    Home,
    Header,
    Swiper,
    SwiperBottom,
    Quotes,
    Footer,
  },
}
</script>

<style scoped>
.v-main {
  display: flex;
  justify-content: space-between;
}

.v-main .vector1 {
  top: 0;
  right: 0;
  position: absolute;
}

.Header {
  position: absolute;
  width: 100%;
}
.hero {
  width: 100%;
  margin-top: 80px;
  display: flex;
  flex-flow: row-reverse;
  justify-content: space-between;
}

.sub-hero1 {
  width: 50%;
}
.sub-hero2 .we-help-you-to-grow {
  margin-top: 50px;
  font-family: 'Hind Vadodara-Bold', Helvetica;
  font-weight: 400;
  color: #331b3b;
  font-size: 87px;
  letter-spacing: -0.87px;
  margin-left: 80px;
  padding: 0;
}
.sub-hero3 {
  width: 515px;
  top: 0;
  margin-left: 80px;
  font-family: 'Hind Vadodara-Regular', Helvetica;
  font-weight: 400;
  color: #331b3ba8;
  font-size: 17px;
  letter-spacing: 0.34px;
}
.sub-hero4 .rectangle {
  width: 207px;
  height: 66px;
  margin-left: 80px;
  background-color: #331b3b;
  border-radius: 10px;
  font-family: 'Hind Vadodara-Bold', Helvetica;
  font-weight: 700;
  color: #ffffff;
  font-size: 17px;
  letter-spacing: 0.34px;
  line-height: 23.3px;
  padding: 20px 0 0 40px;
}
.hero2 {
  width: 100%;
  margin-top: 80px;
  display: flex;
  flex-flow: row;
  justify-content: space-evenly;
}

.sub2-hero1 {
  width: 50%;
}
.sub2-hero2 .we-help-you-to-grow {
  margin-top: 200px;
  margin-left: 80px;
}
.sub2-hero2 .we-help-you-to-grow .text-wrapper {
  line-height: 50px;
  font-family: 'Hind Vadodara', Helvetica;
  font-weight: 700;
  color: #331b3b;
  font-size: 48px;
  word-wrap: break-word;
}
.sub2-hero2 .we-help-you-to-grow .span {
  margin-top: 50px;
  font-family: 'Hind Vadodara', Helvetica;
  font-weight: 300;
  color: #331b3b;
  font-size: 48px;
}
.sub2-hero3 {
  width: 515px;
  top: 0;
  margin-left: 80px;
  font-family: 'Hind Vadodara-Regular', Helvetica;
  font-weight: 400;
  color: #331b3ba8;
  font-size: 17px;
  letter-spacing: 0.34px;
}
.sub2-hero4 .rectangle {
  width: 207px;
  height: 66px;
  margin-left: 80px;
  background-color: #331b3b;
  border-radius: 10px;
  font-family: 'Hind Vadodara-Bold', Helvetica;
  font-weight: 700;

  font-size: 17px;
  letter-spacing: 0.34px;
  line-height: 23.3px;
  padding: 20px 0px 0px 40px;
  margin-top: 40px;
}
.second-swiper {
  width: 100%;
}
</style>
