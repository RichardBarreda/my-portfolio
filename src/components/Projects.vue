<template>
    <div class="project-holder">
      <p class="project-title">Projects</p>
      <p class="project-text">
          With my 3 years of experience as a Web Developer, I already worked with lots of front-end development projects, but unfortunately I cannot disclose
          any information regarding my previous website projects due to the Confidentiality Agreement with my previous employers and with the copyright / code ownership. I can't publicly share the code without the client's permission.
          But to give an idea, I think I've already worked with approximately 11 Web Development Projects.
      </p>
      <p class="project-text">Listed below are some of my sample website projects, with the Nanox Philippines Inc. Company Website as my recent Front-end project.</p>
      <p class="sub-title"> <i class="bi bi-code-slash"></i> Sample Projects:</p>
      <div class="website-wrapper">
        <Website :name="projectName1" :image="projectImage1" :link="projectLink1" :language="projectLanguage1" :description="projectDescription1" :theme="projectTheme1"></Website>
        <Website :name="projectName2" :image="projectImage2" :link="projectLink2" :language="projectLanguage2" :description="projectDescription2" :theme="projectTheme2"></Website>
        <Website :name="projectName3" :image="projectImage3" :link="projectLink3" :language="projectLanguage3" :description="projectDescription3" :theme="projectTheme3"></Website>
        <Website :name="projectName4" :image="projectImage4" :link="projectLink4" :language="projectLanguage4" :description="projectDescription4" :theme="projectTheme4"></Website>
      </div>
      
    </div>
</template>
  



<script>
  import Website from "./Website.vue"
  export default {
    name: 'Projects',
    components: {
      Website
    },
    data() {
        return {
          projectName1: "Nanox Philippines",
          projectImage1: require('../assets/nanox-website.png'),
          projectLink1: "https://nanoxphilippines.com/",
          projectLanguage1: ["HTML", "CSS", "SASS", "JS"],
          projectDescription1: "Company website for Nanox Philippines Inc. Featuring the products and services they offer.",
          projectTheme1: "#1c4175",

          projectName2: "Ticketing System",
          projectImage2: require('../assets/ticketing-system.png'),
          projectLink2: "https://richardbarreda.github.io/ticketing-system/",
          projectLanguage2: ["HTML", "CSS", "VUE", "JS"],
          projectDescription2: "Sample Front-end concept for an IT Department Ticketing System.",
          projectTheme2: "#563d7c",

          projectName3: "My Portfolio",
          projectImage3: require('../assets/portfolio-website.png'),
          projectLink3: "https://richardbarreda.github.io/my-portfolio/",
          projectLanguage3: ["HTML", "CSS", "VUE", "JS"],
          projectDescription3: "My personal space that features my work information, projects, and skills.",
          projectTheme3: "#004D40",

          projectName4: "Cashless Payment System",
          projectImage4: require('../assets/cps-system.png'),
          projectLink4: "",
          projectLanguage4: ["HTML", "CSS", "SASS", "JS", "LARAVEL"],
          projectDescription4: "POS I develop for Nanox to provide Cashless Payment and to avoild physical contact with money due to covid19 pandemic.",
          projectTheme4: "#808080",
        }
    }
  }
</script>
  



<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.project-holder {

}

.project-title {
  font-size: 30px;
  font-weight: 700;
  margin-bottom: 10px;
  text-transform: uppercase;
  color: #0A5C36;
}

.project-text {
  font-size: 18px;
  padding-bottom: 15px;
}

.website-wrapper {
  display: flex;
  flex-wrap: wrap;
  padding-bottom: 30px;
}

.sub-title {
  margin-top: 20px;

  font-size: 20px;
  font-weight: 500;
  text-transform: uppercase;
  color: #0A5C36;
}

@media (min-width: 576px) and (max-width: 767.98px) {
  .project-text {
    font-size: 14px;
  }

  .project-title {
        font-size: 22px;
        margin-bottom: 2px;
    }
}

@media (max-width: 575.98px) {
  .project-text {
    font-size: 14px;
  }

  .project-title {
        font-size: 22px;
        margin-bottom: 2px;
    }  
}
</style>
  