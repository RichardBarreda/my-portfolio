<template>
    <div class="accordion-selector">
        <p class="accordion-link" :class="{active:aboutMeIsActive}" @click="handleAboutMe"> <i class="bi bi-person-badge accordion-icon"></i> <span class="label-text">ABOUT ME</span></p>
        <p class="accordion-link" :class="{active:workHistoryIsActive}" @click="handleWorkHistory"> <i class="bi bi-laptop accordion-icon"></i> <span class="label-text">WORK HISTORY</span></p>
        <p class="accordion-link" :class="{active:projectsIsActive}" @click="handleProjects"> <i class="bi bi-archive accordion-icon"></i> <span class="label-text">PROJECTS</span></p>
        <p class="accordion-link desktop-hidden" :class="{active:moreIsActive}" @click="handleMore"> <i class="bi bi-rocket-takeoff accordion-icon"></i> <span class="label-text">MORE</span></p>
    </div>

    <div class="accordion-information">
        <AboutMe v-if="aboutMeIsActive"></AboutMe>
        <WorkHistory v-if="workHistoryIsActive"></WorkHistory>
        <Projects v-if="projectsIsActive"></Projects>
        <More v-if="moreIsActive"></More>
    </div>
</template>
  



<script>
import AboutMe from "./AboutMe.vue"
import WorkHistory from "./WorkHistory.vue"
import Projects from "./Projects.vue"
import More from "./More.vue"

  export default {
    name: 'Accordion',
    components: {
        AboutMe, WorkHistory, Projects, More
    },
    data() {
        return {
            aboutMeIsActive: true,
            workHistoryIsActive: false,
            projectsIsActive: false,
            moreIsActive: false,
        }
    },
    methods: {
        handleAboutMe() {
            this.aboutMeIsActive = true;
            this.workHistoryIsActive = false;
            this.projectsIsActive = false;
            this.moreIsActive = false;
        },

        handleWorkHistory() {
            this.aboutMeIsActive = false;
            this.workHistoryIsActive = true;
            this.projectsIsActive = false;
            this.moreIsActive = false;
        },

        handleProjects() {
            this.aboutMeIsActive = false;
            this.workHistoryIsActive = false;
            this.projectsIsActive = true;
            this.moreIsActive = false;
        },

        handleMore() {
            this.aboutMeIsActive = false;
            this.workHistoryIsActive = false;
            this.projectsIsActive = false;
            this.moreIsActive = true;
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
    padding-bottom: 10px;
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

.desktop-hidden {
    display: none;
}

.accordion-icon {
    font-size: 20px;
    padding-right: 10px;
}

.accordion-link:hover {
    cursor: pointer;
}

.old-active {

    color: black;
    border-bottom: solid 3px #0A5C36;
    font-weight: 700;

}

.active {
    color: white;
    border-bottom: solid 3px #0A5C36;
    font-weight: 700;
    background-color: #0A5C36;
    border-radius: 10px;
}

.accordion-information {
    box-shadow: 0 3px 6px rgba(0, 0, 0, 0.16), 0 3px 6px rgba(0, 0, 0, 0.23);
    background-color: white;
    border-top: none;
    padding: 30px;
}

@media (max-width: 991.98px) {
    .accordion-selector {
        justify-content: space-around;
    }
}

@media (min-width: 576px) and (max-width: 767.98px) {
    .accordion-link {
        padding: 0px 15px;
        font-size: 14px;
    }

    .desktop-hidden {
        display: flex
    }
}

@media (max-width: 575.98px) {
    .accordion-link {
        padding: 0px 15px;
        font-size: 14px;
        width: 100%;
    }

    .label-text {
        display: none;
    }

    .desktop-hidden {
        display: flex;
    }

    .accordion-icon {
        padding-right: 0px;
    }

    .accordion-information {
        padding: 20px;
    }
}
</style>
  