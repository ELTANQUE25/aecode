<!--
An example of creating a reusable grid component and using it with external data.
-->

<script setup>
// import demogrid from './Grid.vue'
import Logo from './Logo.vue'
import { ref } from 'vue'
import './css/main.css'

</script>

<template>
<Logo class="logo" />

<swiper
    :slides-per-view="1"
    :space-between="50"
    @swiper="onSwiper"
    @slideChange="onSlideChange"
    
  >
    <swiper-slide>
      <div >
        <div class="scritta">
          <h2>Sito Aziendale</h2>
          <p>Creazione siti Web Aziendali e grandi PMI.</p>
        </div>
      <img class='screen' src="https://www.artworkstudios.it/wp-content/uploads/2019/11/web-agency-milano--768x396.png" /> 
      </div>
      </swiper-slide>
    <swiper-slide> </swiper-slide>
    <swiper-slide> </swiper-slide>
    </swiper>


</template>

<script>
  // Import Swiper Vue.js components
  import { Swiper, SwiperSlide } from 'swiper/vue';

  // Import Swiper styles
  import 'swiper/css';

  export default {
    components: {
      Swiper,
      SwiperSlide,
    },
    setup() {
      const onSwiper = (swiper) => {
        console.log(swiper);
      };
      const onSlideChange = () => {
        console.log('slide change');
      };
      return {
        onSwiper,
        onSlideChange,
      };
    },
  };
</script>