<template>
  <div class="main-container">
    <div class="text">
      <div class="left-text">
        <span class="our-recent-work">Our Recent Work<br /></span
        ><span class="by-our-experts">By Our Experts</span>
      </div>
      <div class="right-text">
        Lorem Ipsum has been the industry's standard dummy text ever since the
        1500s, when an unknown printer took a galley of type and scrambled.
      </div>
    </div>
    <div class="container">
      <div class="card"><SecondCard /></div>
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
.container {
  margin-top: 50px;
  margin-left: 25%;
}

.container {
  display: flex;
  flex-wrap: wrap;
}

.text {
  margin: 50px 60px 0px 60px;
  display: flex;
  justify-content: space-evenly;

  font-family: 'Hind Vadodara', sans-serif;
}
.right-text {
  font-family: 'Hind Vadodara', sans-serif;
  width: 100%;
  height: 100%;
  color: #331b3b;
  font-size: 17px;
  font-weight: 400;
  line-height: 24.87px;
  letter-spacing: 0.34px;
  word-wrap: break-word;
}
.left-text {
  display: flex;
  flex-direction: column;
  width: 150%;
}
.our-recent-work {
  color: #331b3b;
  font-size: 48px;
  font-weight: 700;
  line-height: 51.02px;
  word-wrap: break-word;
}
.by-our-experts {
  color: #331b3b;
  font-size: 48px;
  font-weight: 300;
  line-height: 51.02px;
  word-wrap: break-word;
}
</style>
