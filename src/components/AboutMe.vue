<template>
    <div class="about-me">
        <Introduction :title="titleIntro" :text="textIntro"></Introduction>
        <Education :title="titleEducation" :text="textEducation"></Education>
        <Technical :title="titleSkills" :text="textSkills"></Technical>
    </div>
</template>
  



<script>
  import Introduction from './Introduction.vue'
  import Education from './Education.vue'
  import Technical from './Technical.vue'

  export default {
    name: 'AboutMe',
    components: {
      Introduction, Education, Technical
    },
    data() {
        return {
          titleIntro: "ABOUT ME",
          textIntro: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Neque sodales ut etiam sit amet nisl. Sed euismod nisi porta lorem mollis. Congue mauris rhoncus aenean vel elit scelerisque mauris pellentesque pulvinar. Sit amet volutpat consequat mauris. Tincidunt ornare massa eget egestas purus viverra. Molestie nunc non blandit massa enim nec. Id ornare arcu odio ut sem nulla pharetra diam sit. Diam phasellus vestibulum lorem sed risus ultricies tristique nulla. Nibh cras pulvinar mattis nunc sed blandit libero volutpat. Proin sed libero enim sed faucibus turpis in eu mi. Facilisi nullam vehicula ipsum a arcu cursus vitae congue mauris. Auctor eu augue ut lectus arcu bibendum. Elit eget gravida cum sociis natoque penatibus et. Duis tristique sollicitudin nibh sit amet commodo nulla.",
        
          titleEducation: "EDUCATION",
          textEducation: "Tincidunt id aliquet risus feugiat in ante metus dictum at. Nunc congue nisi vitae suscipit tellus mauris a diam maecenas. Fusce ut placerat orci nulla pellentesque dignissim. Maecenas sed enim ut sem viverra aliquet eget sit. Nisl tincidunt eget nullam non nisi est sit amet facilisis. Et odio pellentesque diam volutpat commodo sed egestas egestas fringilla. Neque sodales ut etiam sit amet nisl purus. Amet consectetur adipiscing elit ut aliquam purus. Quis imperdiet massa tincidunt nunc pulvinar sapien. Tellus id interdum velit laoreet id. Pharetra diam sit amet nisl.",

          titleSkills: "PROFESSIONAL SKILLS",
          textSkills: "Tincidunt id aliquet risus feugiat in ante metus dictum at. Nunc congue nisi vitae suscipit tellus mauris a diam maecenas. Fusce ut placerat orci nulla pellentesque dignissim. Maecenas sed enim ut sem viverra aliquet eget sit. Nisl tincidunt eget nullam non nisi est sit amet facilisis.",

        }
    }
  }
</script>
  



<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.skills-wrapper {
  display: flex;
  flex-wrap: wrap;
}
</style>
  