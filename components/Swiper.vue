<script setup lang="ts">
import {Swiper, SwiperSlide} from "swiper/vue";
import { ref } from 'vue';

import "swiper/css"
import 'swiper/swiper-bundle.css';

/*export default {
  components: {
    Swiper,
    SwiperSlide
  },

  data(){
    return{
      photos: ['photo_1.jpg', 'photo_2.jpg', 'photo_3.jpg', 'photo_4.jpg']
    };
  }
};*/

const photos = ref([
  "photo_1.jpg",
  "photo_2.jpg",
  "photo_3.jpg",
  "photo_4.jpg",
  "photo_5.jpg",
]);

</script>

<template>

  <div>
    <h1>Empeereza yaffe</h1>
    <Swiper :space-between="50" :slides-per-view="1">
      <SwiperSlide v-for="(photo, index) in photos" :key="index">
<!--        <img :src="`/assets/images/photo_2.jpg`" alt=""/>-->
        <img :src="`/assets/images/${photo}`" alt="">

      </SwiperSlide>
    </Swiper>
  </div>

  ...

</template>

<style scoped>

</style>