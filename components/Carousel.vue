<template>
  <swiper
    :spaceBetween="30"
    :centeredSlides="true"
    :autoplay="{
      delay: 2500,
      disableOnInteraction: false,
    }"
    :pagination="{
      clickable: true,
    }"
    :navigation="true"
    :modules="modules"
    class="mySwiper"
  >
    <swiper-slide>
      <img
        className="object-fill w-full h-96"
        src="https://res.cloudinary.com/lamcom/image/upload/v1671026502/santhibakery/slider/slider-1_mvhocx.jpg"
        alt="image slide 1"
      />
      <div class="relative max-w-7xl -mt-64 px-24">
        <div class="absolute mx-auto justify-center">
          <p class="text-5xl font-extrabold text-white text-left uppercase">
            Cakes
          </p>
          <p
            class="text-2xl font-semibold text-white text-left leading-10 py-2"
          >
            Always Fress and Always Delicious
          </p>
          <p class="text-md font-normal text-white text-left leading-5">
            Santhi Bakery, Tiruchendur, are reputed bakers whose cakes are
            delicious and tasty.<br />They make a variety of cakes, suitable for
            Birthday, Anniversary, Festivals and all other occasions.
          </p>
        </div>
      </div>
    </swiper-slide>
    <swiper-slide>
      <img
        className="object-fill w-full h-96"
        src="https://res.cloudinary.com/lamcom/image/upload/v1671026768/santhibakery/slider/slider-2_e5hfff.jpg"
        alt="image slide 2"
      />
       <div class="relative max-w-7xl -mt-64 px-24">
      <div class="absolute mx-auto justify-center w-full">
        <p class="text-5xl font-extrabold text-white text-left uppercase">
          Macroon
        </p>
        <p
          class="text-2xl font-semibold text-white text-left leading-10 py-2"
        >
          Always Fress and Always Delicious
        </p>
        <p class="text-md font-normal text-white text-left leading-5">
          Macaroons are made with cashew nuts as major ingredient in the
          Tuticorin District, <br />For quality-wise and taste-wise, our Macaroons are
          the best in Tiruchendur and neighbouring areas.
        </p>
      </div>
       </div>
    </swiper-slide>
    <swiper-slide>
      <img
        className="object-fill w-full h-96"
        src="https://res.cloudinary.com/lamcom/image/upload/v1671027210/santhibakery/slider/slider-3_jz0869.jpg"
        alt="image slide 3"
      />
      
      <div class="absolute mx-auto justify-center w-full -mt-56 lg:px-24">
        <p class="lg:text-5xl md:text-xl font-extrabold text-white text-left uppercase">
          Welcome to Santhi Bakery
        </p>
        <p class="lg:text-2xl md:text-xl font-semibold text-white text-left leading-10">
          Always Fress and Always Delicious
        </p>
          <p class="text-md font-normal text-white text-left leading-5">
            Santhi Bakery, Tiruchendur, are reputed bakers whose cakes are
            delicious and tasty.<br />They make a variety of cakes, suitable for
            Birthday, Anniversary, Festivals and all other occasions.
          </p>
      </div>
    </swiper-slide>
  </swiper>
</template>

<script>
// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from "swiper/vue";

// Import Swiper styles
import "swiper/css";

import "swiper/css/pagination";
import "swiper/css/navigation";

// import required modules
import { Autoplay, Pagination, Navigation } from "swiper";

export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    return {
      modules: [Autoplay, Pagination, Navigation],
    };
  },
};
</script>