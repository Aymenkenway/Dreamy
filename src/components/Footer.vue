<template>
  <div class="main-container">
    <div class="text">
      <div class="left-text">
        <div class="first-quote">
          <div class="dream-agency">Dream Agency</div>
          <div class="lorem">
            Lorem Ipsum has been the industry's standard dummy text ever since
            the 1500s, when an unknown printer took a galley of type and
            scrambled it to make a type specimen book. It has survived not only
            five centuries.
          </div>

          <div class="get-in-touch">GET IN TOUCH</div>
          <img class="button-section" src="../assets/icons/button.png" alt="" />
        </div>
      </div>
      <div class="right-text">
        <img src="../assets/icons/map.png" alt="" />
      </div>
    </div>
  </div>
</template>

<script>
import SecondCard from './SecondCard.vue'

export default {
  components: {
    SecondCard,
  },
  data: () => ({
    //
  }),
}
</script>

<style scoped>
@import '../assets/fonts/fonts.css';
.main-container {
  padding-top: 40px;
  display: flex;
  justify-content: space-between;
  margin-top: 50px;
  width: 100%;
  height: 100%;
  border-top-right-radius: 158px;
  background-color: black;
}

.dream-agency {
  color: white;
  font-size: 50px;
  font-family: Playfair Display;
  font-weight: 700;
  letter-spacing: 0.36px;
  word-wrap: break-word;
}
.lorem {
  color: white;
  font-size: 16px;
  font-family: 'Hind Vadodara', sans-serif;
  font-weight: 400;
  line-height: 25.49px;
  letter-spacing: 0.32px;
  word-wrap: break-word;
}
.get-in-touch {
  color: white;
  font-size: 16px;
  font-family: 'Hind Vadodara', sans-serif;
  font-weight: 600;
  text-transform: uppercase;
  line-height: 25.49px;
  letter-spacing: 0.32px;
  word-wrap: break-word;
  padding: 10px 0px 10px 0px;
}
.button-section {
  width: 400px;
}
.text {
  margin: 50px 60px 0px 60px;
  display: flex;
  justify-content: space-evenly;

  font-family: 'Hind Vadodara', sans-serif;
}
.right-text {
  width: 100%;
}
.left-text {
  display: flex;
  flex-direction: column;
  width: 100%;
  padding-right: 20%;
}
</style>
