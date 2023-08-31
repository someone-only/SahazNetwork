<script setup lang="ts">
import { ref } from "vue";
import { SwiperSlide, Swiper } from "swiper/vue";
import { Pagination, EffectFade, Autoplay } from "swiper/modules";
import "swiper/css";
import "swiper/css/pagination";
import "swiper/css/effect-fade";

const modules = ref([Pagination, EffectFade, Autoplay]);
</script>
<template>
  <Swiper
    :autoplay="{
      delay: 10000,
    }"
    :modules="modules"
    :pagination="{ clickable: true }"
    :slides-per-view="1"
    :space-between="50"
    effect="fade"
    class="w-full h-full"
    style="width: 100%; height: 300px"
  >
    <SwiperSlide>
      <img
        src="https://source.unsplash.com/400x300?internet"
        alt=""
        class="w-full h-full object-cover"
      />
    </SwiperSlide>
    <SwiperSlide>
      <img
        src="https://source.unsplash.com/400x300?world"
        alt=""
        class="w-full h-full object-cover"
      />
    </SwiperSlide>
    <SwiperSlide>
      <img
        src="https://source.unsplash.com/400x300?sea"
        alt=""
        class="w-full h-full object-cover"
      />
    </SwiperSlide>
    <SwiperSlide>
      <img
        src="https://source.unsplash.com/400x300?greenland"
        alt=""
        class="w-full h-full object-cover"
      />
    </SwiperSlide>
  </Swiper>
</template>
