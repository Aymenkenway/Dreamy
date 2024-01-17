<template>
  <div class="v-app-bar">
    <ul class="links">
      <li>Home</li>
      <li>About US</li>
      <li>Services</li>
      <li>Contact Us</li>
    </ul>
    <div class="brand-text">Dream Agency</div>
    <div class="icons">
      <div class="container">
        <img src="../assets//icons/facebook.png" alt="Facebook" />
      </div>
      <div class="container">
        <img src="../assets/icons/linkedin.svg" alt="Instagram" />
      </div>
      <div class="container">
        <img src="../assets/icons/instagram.svg" alt="LinkedIn" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Header',

  components: {},

  data: () => ({
    //
  }),
}
</script>

<style scoped>
.brand-text {
  width: 33%;
  color: #331b3b;
  font-size: 24px;
  font-family: Playfair Display;
  font-weight: 700;
  letter-spacing: 0.24px;
  display: flex;
  justify-content: center;
}
.v-app-bar {
  display: flex;
  justify-content: space-between;

  margin: 30px 20px 0px 20px;
}

.links {
  margin-top: 10px;
  list-style: none;
  display: flex;
  justify-content: space-evenly;
  width: 33%;
  color: #331b3b;
  font-size: 16px;
  font-style: normal;
  line-height: normal;
  letter-spacing: 0.16px;
}
.single-link {
  border-radius: 174px 117px 165px 116px;
  -webkit-border-radius: 174px 117px 165px 116px;
  -moz-border-radius: 174px 117px 165px 116px;
  border: 2px solid #000000;
}

.icons {
  mask-position: absolute;
  display: flex;
  justify-content: flex-end;
  align-items: baseline;
  width: 33%;
}

.icons .container {
  padding: 0;
  border-radius: 60%;
  margin: 0 10px 0 10px;
  width: 43.61px;
  height: 49.61px;
  left: 1200.61px;
  top: 26.36px;
  transform: rotate(30.5deg);
  transform-origin: 20px 0;
  border: 2px rgba(51, 27, 59, 0.64) solid;
}
.container img {
  margin: 10px 0 0 10px;
  transform: rotate(330deg);
}
</style>
