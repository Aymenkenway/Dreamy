<template>
  <div>
    <swiper
      :slides-per-view="5"
      :space-between="70"
      :loop="false"
      :pagination="true"
      :navigation="true"
      @swiper="onSwiper"
      @slideChange="onSlideChange"
    >
      <swiper-slide
        v-for="(slide, index) in slides"
        :key="index"
        class="test"
        :class="{ test_2: true }"
      >
        <div class="box">
          <div class="rectangle">
            <div class="small-box">
              <div
                class="small-rectangle"
                :style="{ backgroundImage: `url(${slide.image})` }"
              ></div>
            </div>
            <h1 class="title">{{ slide.title }}</h1>
            <p class="lorem">
              {{ slide.text }}
            </p>
          </div>
        </div>
      </swiper-slide>
    </swiper>
  </div>
</template>

<script>
import SwiperCore, { Navigation, Pagination } from 'swiper'
import { Swiper, SwiperSlide } from 'swiper/vue'

import 'swiper/swiper-bundle.css'

SwiperCore.use([Navigation, Pagination])

export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  data() {
    return {
      slides: [
        {
          title: 'WEBSITE DESIGN',
          text: 'Lorem ipsum dolor sit, amet consectetur adipisicing elit. A asperiores error eum laboriosam. Illo, quidem? Distinctio deserunt error',
          image: require('../assets/icons/website.png'),
        },
        {
          title: 'WEB DEVELOPMENT',
          text: 'Lorem ipsum dolor sit, amet consectetur adipisicing elit. A asperiores error eum laboriosam. Illo, quidem? Distinctio deserunt error',
          image: require('../assets/icons/computer.png'),
        },
        {
          title: 'MOBILE APP DEVELOPMENT',
          text: 'Lorem ipsum dolor sit, amet consectetur adipisicing elit. A asperiores error eum laboriosam. Illo, quidem? Distinctio deserunt error',
          image: require('../assets/icons/mobile.png'),
        },
        {
          title: 'MARKETING',
          text: 'Lorem ipsum dolor sit, amet consectetur adipisicing elit. A asperiores error eum laboriosam. Illo, quidem? Distinctio deserunt error',
          image: require('../assets/icons/rocket.png'),
        },
        {
          title: 'WEBSITE DESIGN',
          text: 'Lorem ipsum dolor sit, amet consectetur adipisicing elit. A asperiores error eum laboriosam. Illo, quidem? Distinctio deserunt error',
          image: require('../assets/icons/website.png'),
        },
      ],
    }
  },
  methods: {
    onSwiper(swiper) {
      console.log(swiper)
    },
    onSlideChange() {
      console.log('slide change')
    },
  },
}
</script>

<style lang="scss" scoped>
.box {
  padding: 10px 0px 40px 10px;
  display: flex;
  justify-content: space-between;
  text-align: left;
}

.box .rectangle {
  width: 308px;
  height: 192px;
  top: 0;
  left: 0;
  border-radius: 10px;
  box-shadow: 0px 0px 9px 2px rgba(0, 0, 0, 0.05);
  padding: 10px 0px 0px 10px;
}
.small-box {
  width: 52px;
  height: 48px;
}

.small-box .small-rectangle {
  display: flex;
  align-items: center;
  justify-content: center;
  position: relative;
  width: 52px;
  height: 48px;
  top: 0;
  left: 0;
  background-color: #ffded4;
  border-radius: 10px;
  background-image: url(../assets/icons/website.png);
  background-position: center;
}
.lorem {
  color: #331b3b;
  font-size: 15px;
  font-weight: 300;
  letter-spacing: 0.3px;
  line-height: 21.8px;
  width: 275px;
  height: 82px;
  font-family: 'Hind Vadodara-Light', sans-serif;
}
.title {
  margin: 10px 0 10px 0;
  color: #331b3b;
  font-size: 2px;
  font-weight: 700;
  letter-spacing: 0.88px;
  left: 0;
  top: 0;
  line-height: 21.8px;
  font-family: 'Hind Vadodara', sans-serif;
  white-space: nowrap;
}
</style>
