
<script setup>
// import demogrid from './Grid.vue'
import Logo from './Logo.vue'
import { ref } from 'vue'
import './css/main.css'

</script>

<template>
<Logo class="logo" />

<swiper
   :pagination="{
      type: 'progressbar',
    }"
    :navigation="true"
    
 
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

<!--
An example of creating a reusable grid component and using it with external data.
-->
<script>
// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from "swiper/vue";

// Import Swiper styles
import "swiper/css";

import "swiper/css/pagination";
import "swiper/css/navigation";


// import required modules
import { Pagination, Navigation } from "swiper";

export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    return {
      modules: [Pagination, Navigation],
    };
  },
};
</script>