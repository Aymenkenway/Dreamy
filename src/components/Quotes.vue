<template>
  <div class="container">
    <div class="text">
      <span class="what-we-do">What We Do<br /></span
      ><span class="for-you-business">For Your Business</span>
    </div>

    <div class="quotes">
      <div class="first-quote">
        <img src="../assets/icons/quote.png" alt="quote" />
        <div class="lorem">
          Lorem Ipsum has been the industry's standard dummy text ever since the
          1500s, when an unknown printer took a galley of type and scrambled it
          to make a type specimen book. It has survived not only five centuries.
        </div>

        <div
          style="
            color: black;
            font-size: 16px;
            font-family: Hind Vadodara;
            font-weight: 600;
            line-height: 25.49px;
            letter-spacing: 0.32px;
            word-wrap: break-word;
          "
        >
          UI Soup
        </div>
      </div>
      <div class="first-quote">
        <img src="../assets/icons/quote.png" alt="quote" />
        <div class="lorem">
          Lorem Ipsum has been the industry's standard dummy text ever since the
          1500s, when an unknown printer took a galley of type and scrambled it
          to make a type specimen book. It has survived not only five centuries.
        </div>

        <div
          style="
            color: black;
            font-size: 16px;
            font-family: Hind Vadodara;
            font-weight: 600;
            line-height: 25.49px;
            letter-spacing: 0.32px;
            word-wrap: break-word;
          "
        >
          UI Soup
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.container .text {
  font-family: monospace;
  font-size: 20px;
  text-align: center;
  display: flex;
  align-items: center;
  height: 200px;
}

.container {
  margin-top: 150px;
  margin-bottom: 100px;
}

.container {
  display: flex;
  flex-wrap: wrap;
  max-width: 1000px;
  margin-left: 20%;
}

.text {
  flex-basis: 100%;
  display: flex;
  flex-direction: column;
}

.what-we-do {
  color: #331b3b;
  font-size: 48px;
  font-family: 'Hind Vadodara-Bold', sans-serif;
  font-weight: 700;
  line-height: 51.02px;
  word-wrap: break-word;
}

.for-you-business {
  color: #331b3b;
  font-size: 48px;
  font-family: 'Hind Vadodara-Light', sans-serif;
  font-weight: 300;
}
.quotes {
  width: 100%;
  display: flex;
  justify-content: space-between;
  flex-flow: row;
}
.quotes .first-quote {
  display: flex;
  margin-right: 30px;
  justify-content: flex-start;
  flex-direction: column;
  text-align: left;
  width: 100%;
  height: 100%;
  background: white;
  box-shadow: 0px 0px 7px 1px rgba(0, 0, 0, 0.08);
}

.first-quote img {
  width: 50px;
  height: auto;
}
.first-quote .lorem {
  color: #331b3b;
  font-size: 16px;
  font-family: 'Hind Vadodara', sans-serif;
  font-weight: 400;
  line-height: 25.49px;
  letter-spacing: 0.32px;
  word-wrap: break-word;
  max-width: 90%;
}
@media only screen and (max-width: 400px) {
  .container .text {
    font-family: monospace;
    font-size: 20px;
    text-align: center;
    display: flex;
    align-items: center;
    height: 200px;
  }

  .container {
    margin-top: 150px;
    margin-bottom: 100px;
  }

  .container {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    max-width: 100%;
    margin-left: 20%;
    margin: 0;
  }

  .text {
    flex-basis: 100%;
    display: flex;
    flex-direction: column;
  }

  .what-we-do {
    color: #331b3b;
    font-size: 48px;
    font-family: 'Hind Vadodara-Bold', sans-serif;
    font-weight: 700;
    line-height: 51.02px;
    word-wrap: break-word;
  }

  .for-you-business {
    color: #331b3b;
    font-size: 48px;
    font-family: 'Hind Vadodara-Light', sans-serif;
    font-weight: 300;
  }
  .quotes {
    width: 100%;
    display: flex;
    justify-content: center;
    flex-flow: column;
    align-items: center;
  }
  .quotes .first-quote {
    display: flex;
    justify-content: center;
    flex-direction: column;
    margin-left: 10%;
    text-align: left;
    width: 70%;
    background: white;
    box-shadow: 0px 0px 7px 1px rgba(0, 0, 0, 0.08);
  }

  .first-quote img {
    width: 50px;
    height: auto;
  }
  .first-quote .lorem {
    color: #331b3b;
    font-size: 16px;
    font-family: 'Hind Vadodara', sans-serif;
    font-weight: 400;
    line-height: 25.49px;
    letter-spacing: 0.32px;
    word-wrap: break-word;
    max-width: 90%;
  }
}
</style>
