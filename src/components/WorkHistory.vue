<template>
    <div class="work-history">
      <Work :company="workCompany1" :date="workDate1" :position="workPosition1">

        <template v-slot:bullet>
          <ul>
            <li class="bullet-items">Tincidunt vitae semper quis lectus nulla at. Nulla posuere sollicitudin aliquam ultrices sagittis orci a scelerisque.</li>
            <li class="bullet-items">Sagittis purus sit amet volutpat consequat mauris nunc. Eleifend mi in nulla posuere sollicitudin aliquam.</li>
            <li class="bullet-items">Viverra suspendisse potenti nullam ac tortor vitae purus faucibus. </li>
            <li class="bullet-items">Varius vel pharetra vel turpis nunc eget. Eu augue ut lectus arcu bibendum at varius vel pharetra.</li>
            <li class="bullet-items">Mus mauris vitae ultricies leo integer malesuada nunc. Lorem ipsum dolor sit amet consectetur adipiscing elit duis.</li>
            <li class="bullet-items">Orci dapibus ultrices in iaculis nunc sed. Consequat interdum varius sit amet mattis vulputate enim.</li>
            <li class="bullet-items">Sit amet risus nullam eget. Arcu dui vivamus arcu felis bibendum ut tristique et egestas. Enim facilisis gravida neque convallis a cras semper.</li>
            <li class="bullet-items">Volutpat sed cras ornare arcu. Arcu ac tortor dignissim convallis aenean. </li>
            <li class="bullet-items">Fringilla phasellus faucibus scelerisque eleifend donec pretium vulputate sapien nec. Dui id ornare arcu odio ut sem nulla.</li>
            <li class="bullet-items">Dapibus ultrices in iaculis nunc sed augue. Mi quis hendrerit dolor magna eget est lorem. Ultricies leo integer malesuada nunc vel risus commodo.</li>
          </ul>
          
        </template>

      </Work>

      <Work :company="workCompany2" :date="workDate2" :position="workPosition2">

        <template v-slot:bullet>
          <ul>
            <li class="bullet-items">Tincidunt vitae semper quis lectus nulla at. Nulla posuere sollicitudin aliquam ultrices sagittis orci a scelerisque.</li>
            <li class="bullet-items">Sagittis purus sit amet volutpat consequat mauris nunc. Eleifend mi in nulla posuere sollicitudin aliquam.</li>
            <li class="bullet-items">Viverra suspendisse potenti nullam ac tortor vitae purus faucibus. </li>
            <li class="bullet-items">Varius vel pharetra vel turpis nunc eget. Eu augue ut lectus arcu bibendum at varius vel pharetra.</li>
            <li class="bullet-items">Mus mauris vitae ultricies leo integer malesuada nunc. Lorem ipsum dolor sit amet consectetur adipiscing elit duis.</li>
            <li class="bullet-items">Orci dapibus ultrices in iaculis nunc sed. Consequat interdum varius sit amet mattis vulputate enim.</li>
            <li class="bullet-items">Sit amet risus nullam eget. Arcu dui vivamus arcu felis bibendum ut tristique et egestas. Enim facilisis gravida neque convallis a cras semper.</li>
            <li class="bullet-items">Volutpat sed cras ornare arcu. Arcu ac tortor dignissim convallis aenean. </li>
            <li class="bullet-items">Fringilla phasellus faucibus scelerisque eleifend donec pretium vulputate sapien nec. Dui id ornare arcu odio ut sem nulla.</li>
            <li class="bullet-items">Dapibus ultrices in iaculis nunc sed augue. Mi quis hendrerit dolor magna eget est lorem. Ultricies leo integer malesuada nunc vel risus commodo.</li>
          </ul>
          
        </template>

      </Work>
    </div>
</template>
  



<script>
  import Work from "./Work.vue"
  export default {
    name: 'WorkHistory',
    components: {
      Work
    },
    data() {
        return {
          workCompany1: "Auctor eu augue",
          workDate1: "Sqxcse 2024 - Tgcrfxsop 2024",
          workPosition1: "tfc qwsdcvghy",

          workCompany2: "Porta non pulvinar neque",
          workDate2: "ogexs 2020 - csxafeht 2023",
          workPosition2: "tgvrfcedxoiu",
        }
    }
  }
</script>
  



<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
  