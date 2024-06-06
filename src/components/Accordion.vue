<template>
    <div class="accordion-selector">
        <p class="accordion-link" :class="{active:aboutMeIsActive}" @click="handleAboutMe"> <i class="bi bi-person-badge accordion-icon"></i> ABOUT ME</p>
        <p class="accordion-link" :class="{active:workHistoryIsActive}" @click="handleWorkHistory"> <i class="bi bi-laptop accordion-icon"></i> WORK HISTORY</p>
        <p class="accordion-link" :class="{active:projectsIsActive}" @click="handleProjects"> <i class="bi bi-archive accordion-icon"></i> PROJECTS</p>
    </div>

    <div class="accordion-information">
        <AboutMe v-if="aboutMeIsActive"></AboutMe>
        <WorkHistory v-if="workHistoryIsActive"></WorkHistory>
        <Projects v-if="projectsIsActive"></Projects>
    </div>
</template>
  



<script>
import AboutMe from "./AboutMe.vue"
import WorkHistory from "./WorkHistory.vue"
import Projects from "./Projects.vue"

  export default {
    name: 'Accordion',
    components: {
        AboutMe, WorkHistory, Projects
    },
    data() {
        return {
            aboutMeIsActive: true,
            workHistoryIsActive: false,
            projectsIsActive: false,
        }
    },
    methods: {
        handleAboutMe() {
            this.aboutMeIsActive = true;
            this.workHistoryIsActive = false;
            this.projectsIsActive = false;
        },

        handleWorkHistory() {
            this.aboutMeIsActive = false;
            this.workHistoryIsActive = true;
            this.projectsIsActive = false;
        },

        handleProjects() {
            this.aboutMeIsActive = false;
            this.workHistoryIsActive = false;
            this.projectsIsActive = true;
        }

    }
  }
</script>
  



<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.accordion-selector {
    display: flex;
    justify-content: flex-start;
    align-items: center;
    margin-top: 15px;
    border-bottom: solid 2px gainsboro;
}

.accordion-link {
    padding: 0px 30px;
    display: flex;
    justify-content: center;
    align-items: center;
    border-bottom: solid 2px transparent;
    height: 45px;
    font-size: 15px;
    font-weight: 700;
    color: #939393;
}

.accordion-icon {
    font-size: 20px;
    padding-right: 10px;
}

.accordion-link:hover {
    cursor: pointer;
    color: gray;
}

.active {
    color: black;
    border-bottom: solid 3px #0A5C36;
    font-weight: 700;
}

.accordion-information {
    
    background-color: white;
    border-top: none;
    padding: 30px;
}
</style>
  