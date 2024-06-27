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
          textIntro: "Hi there! I am Richard Marck Barreda. An IT Specialist and Web developer from Angeles City Pampanga, Philippines. As an IT Specialist I have an experience working on Technical Support Industry wherein I was able to provide technical assistance to employees who are experiencing issues with their computer whether it is a hardware or software problem. I am also a Web developer that specialized in front-end development. I have an approximately 3 years of experience on web development, part of those experience were the knowledge and skills I gain to be a front-end developer from my first company and the experience I gain from my current company wherein I was able to explore the side of a back-end developer. My ultimate goal as a web developer is to become a full-fledged Full-Stack Developer. I know that there will be alot of challenges along my way but I am standing confident, because I am dedicated and eager to learn new technologies and frameworks to stay current in this ever-evolving field.",
        
          titleEducation: "EDUCATION",
          textEducation: "Tincidunt id aliquet risus feugiat in ante metus dictum at. Nunc congue nisi vitae suscipit tellus mauris a diam maecenas. Fusce ut placerat orci nulla pellentesque dignissim. Maecenas sed enim ut sem viverra aliquet eget sit. Nisl tincidunt eget nullam non nisi est sit amet facilisis. Et odio pellentesque diam volutpat commodo sed egestas egestas fringilla. Neque sodales ut etiam sit amet nisl purus. Amet consectetur adipiscing elit ut aliquam purus. Quis imperdiet massa tincidunt nunc pulvinar sapien. Tellus id interdum velit laoreet id. Pharetra diam sit amet nisl.",

          titleSkills: "PROFESSIONAL SKILLS",
          textSkills: "",

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
  