<template>
  <div class="container">
    <div class="text">
      <span class="what-we-do">What We Do<br /></span
      ><span class="for-you-business">For Your Business</span>
    </div>

    <div class="card"><Card /></div>
  </div>
</template>

<script>
import Card from './Card.vue'

export default {
  name: 'Header',
  components: {
    Card,
  },
  data: () => ({
    //
  }),
}
</script>

<style scoped>
.container div {
  font-family: monospace;
  font-size: 20px;
  text-align: center;
  display: flex;
  align-items: center;
  height: 200px;

  margin-left: 10%;
}

.container {
  margin-top: 10%;
}

.container {
  display: flex;
  flex-wrap: wrap;
}

.text {
  flex-basis: 100%;
  display: flex;
  flex-direction: column;
}

.card {
  flex: 3;
}

.what-we-do {
  color: #331b3b;
  font-size: 48px;
  font-family: 'Hind Vadodara-Bold', Helvetica;
  font-weight: 700;
  line-height: 51.02px;
  word-wrap: break-word;
}

.for-you-business {
  color: #331b3b;
  font-size: 48px;
  font-family: 'Hind Vadodara-Light', Helvetica;
  font-weight: 300;
}
</style>
