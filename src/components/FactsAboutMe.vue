<template>
    <div class="facts-holder">
        <p class="section-title">FACTS ABOUT ME</p>
        <swiper :navigation="true" :loop="true" :space-between="50" :autoplay="{ delay: 8500, disableOnInteraction: false,}" :modules="modules" class="mySwiper fact-swiper">
            <p class="section-title">FACTS ABOUT ME</p>
            <swiper-slide v-for="fact in content" :key="fact.key">
                <div class="content-holder">
                    <div class="banner-holder">
                        <img :src="fact.banner" class="fact-image" />
                    </div>
                    <div class="details-holder">
                        <p class="fact-title">{{fact.title}}</p>
                        <p class="fact-text">{{fact.content}}</p>
                    </div>
                </div>
            </swiper-slide>
        </swiper>
    </div>
</template>
  



<script>
// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from 'swiper/vue';

// Import Swiper styles
import 'swiper/css';
import 'swiper/css/navigation';


// import required modules
import { Autoplay, Navigation } from 'swiper/modules';

export default {
    name: 'Facts',
    components: {
      Swiper,
      SwiperSlide,
    },
    props:["content"],
    setup() {
      return {
        modules: [Autoplay, Navigation],
      };
    },
    data() {
        return {

        }
    }
}
</script>
  



<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.facts-holder {
    width: 100%;
    max-width: 100%;
    
    border-radius: 3px;
    background-color: whitesmoke;
    margin-bottom: 30px;

    position: relative;
    box-shadow: 0 3px 6px rgba(0, 0, 0, 0.16), 0 3px 6px rgba(0, 0, 0, 0.23);
}
.banner-holder {
    height: 200px;
    position: relative;
}

.section-title {
    position: absolute;
    font-size: 14px;
    font-weight: 500;
    color: black;
    background-color: #ffffffa8;
    top: 5px;
    left: 5px;
    padding: 3px 10px;
    z-index: 1;
}

.fact-image {
    width: 100%;
    max-width: 100%;
    height: 100%;
    object-fit: cover;
}

.details-holder {
    height: 200px;
    padding: 15px;
}

.fact-title {
    font-size: 18px;
    font-weight: 500;
    color: black;

}

.fact-text {
    font-size: 14px;
    line-height: 20px;
    color: #575757;
}

</style>
  