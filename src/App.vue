<template>
  <Header></Header>
  <Body></Body>
</template>

<script>
import Header from './components/Header.vue'
import Body from './components/Body.vue'


export default {
  name: 'App',
  components: {
    Header, Body
  }
}
</script>

<style>

.custom-container {
  width: 100%;
  max-width: 100%;
  padding: 0px 30px;
}

p {
  padding: 0px;
  margin: 0px
}

.fact-swiper .swiper-button-prev,
.fact-swiper .swiper-button-next {
    margin-top: -55px;
    background-color: #f5f5f5e0;
    border-radius: 10px;
    height: auto;
    padding: 10px;

    opacity: .6;
}

.fact-swiper .swiper-button-prev:hover,
.fact-swiper .swiper-button-next:hover {
    opacity: 1;
}

.fact-swiper .swiper-button-prev:after,
.fact-swiper .swiper-button-next:after {
    font-size: 18px;
    color: black;
    font-weight: 800;
}

@media (min-width: 992px) and (max-width: 1199.98px) {
  .fact-swiper .swiper-button-prev,
  .fact-swiper .swiper-button-next {
      margin-top: -80px;
  }    
}

@media (max-width: 575.98px) {
  .custom-container {
    padding: 0px 15px;
  }  
  
  .fact-swiper .swiper-button-prev,
  .fact-swiper .swiper-button-next {
      margin-top: -70px;
  } 
}

</style>
