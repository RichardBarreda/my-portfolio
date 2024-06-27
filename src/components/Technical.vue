<template>
    <div class="technical-holder">
        <p class="technical-title">{{title}}</p>
        <p class="technical-text">
            {{text}}
        </p>

        <div class="skill-group">
            <p class="sub-title"><i class="bi bi-code-slash"></i> Technical</p>
            <div class="skills-wrapper">
                <Skills :name="skillName1" :icon="skillIcon1" :level="skillLevel1"></Skills>
                <Skills :name="skillName2" :icon="skillIcon2" :level="skillLevel2"></Skills>
                <Skills :name="skillName3" :icon="skillIcon3" :level="skillLevel3"></Skills>
                <Skills :name="skillName4" :icon="skillIcon4" :level="skillLevel4"></Skills>
                <Skills :name="skillName5" :icon="skillIcon5" :level="skillLevel5"></Skills>
                <Skills :name="skillName6" :icon="skillIcon6" :level="skillLevel6"></Skills>
                <Skills :name="skillName13" :icon="skillIcon13" :level="skillLevel13"></Skills>
                <Skills :name="skillName7" :icon="skillIcon7" :level="skillLevel7"></Skills>
                <Skills :name="skillName8" :icon="skillIcon8" :level="skillLevel8"></Skills>
                <Skills :name="skillName9" :icon="skillIcon9" :level="skillLevel9"></Skills>
                <Skills :name="skillName10" :icon="skillIcon10" :level="skillLevel10"></Skills>
                <Skills :name="skillName11" :icon="skillIcon11" :level="skillLevel11"></Skills>
                <Skills :name="skillName12" :icon="skillIcon12" :level="skillLevel12"></Skills>
            </div>
        </div>

        <div class="skill-group">
            <p class="sub-title"><i class="bi bi-journal-richtext"></i> Personal</p>
            <div class="skills-wrapper">
                <Skills :name="personalSkill1" :icon="personalIcon1" :level="personalLevel1"></Skills>
                <Skills :name="personalSkill2" :icon="personalIcon2" :level="personalLevel2"></Skills>
                <Skills :name="personalSkill3" :icon="personalIcon3" :level="personalLevel3"></Skills>
                <Skills :name="personalSkill4" :icon="personalIcon4" :level="personalLevel4"></Skills>
                <Skills :name="personalSkill5" :icon="personalIcon5" :level="personalLevel5"></Skills>
                <Skills :name="personalSkill6" :icon="personalIcon6" :level="personalLevel6"></Skills>
                <Skills :name="personalSkill7" :icon="personalIcon7" :level="personalLevel7"></Skills>
                <Skills :name="personalSkill8" :icon="personalIcon8" :level="personalLevel8"></Skills>
                <Skills :name="personalSkill9" :icon="personalIcon9" :level="personalLevel9"></Skills>
            </div>
        </div>
        
        
    </div>
</template>
  



<script>
  import Skills from "./Skill.vue"
  export default {
    name: 'Technical',
    props: ["title", "text"],
    components: {
        Skills
    },
    data() {
        return {
            skillName1: "HTML",
            skillIcon1: require('../assets/html.png'),
            skillLevel1: "90%",

            skillName2: "CSS",
            skillIcon2: require('../assets/css-3.png'),
            skillLevel2: "90%",

            skillName3: "Javascript",
            skillIcon3: require('../assets/js.png'),
            skillLevel3: "70%",

            skillName4: "SASS",
            skillIcon4: require('../assets/sass.png'),
            skillLevel4: "90%",

            skillName5: "Bootstrap",
            skillIcon5: require('../assets/bootstrap.png'),
            skillLevel5: "90%",

            skillName6: "VUE",
            skillIcon6: require('../assets/vue.png'),
            skillLevel6: "65%",

            skillName7: "PHP",
            skillIcon7: require('../assets/php.png'),
            skillLevel7: "25%",

            skillName8: "LARAVEL",
            skillIcon8: require('../assets/laravel.png'),
            skillLevel8: "50%",

            skillName9: "JAVA",
            skillIcon9: require('../assets/java.png'),
            skillLevel9: "20%",

            skillName10: "Python",
            skillIcon10: require('../assets/python.png'),
            skillLevel10: "15%",

            skillName11: "C#",
            skillIcon11: require('../assets/c-sharp.png'),
            skillLevel11: "20%",

            skillName12: "C++",
            skillIcon12: require('../assets/c-pp.png'),
            skillLevel12: "15%",

            skillName13: "REACT",
            skillIcon13: require('../assets/react.png'),
            skillLevel13: "20%",





            personalSkill1: "Time Management",
            personalIcon1: require('../assets/time.png'),
            personalLevel1: "70%",

            personalSkill2: "Creative",
            personalIcon2: require('../assets/creative.png'),
            personalLevel2: "75%",

            personalSkill3: "Analytical Skills",
            personalIcon3: require('../assets/analytical.png'),
            personalLevel3: "70%",

            personalSkill4: "Communication",
            personalIcon4: require('../assets/communication.png'),
            personalLevel4: "75%",

            personalSkill5: "Teamwork",
            personalIcon5: require('../assets/team.png'),
            personalLevel5: "90%",

            personalSkill6: "Organizational Skill",
            personalIcon6: require('../assets/organizational.png'),
            personalLevel6: "75%",

            personalSkill7: "Flexible",
            personalIcon7: require('../assets/attention.png'),
            personalLevel7: "70%",

            personalSkill8: "Problem Solving",
            personalIcon8: require('../assets/solving.png'),
            personalLevel8: "70%",

            personalSkill9: "Leadership",
            personalIcon9: require('../assets/leader.png'),
            personalLevel9: "60%",
        }
    }
  }
</script>
  



<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.technical-holder {
    padding-bottom: 30px;
}

.technical-title {
    font-size: 30px;
    font-weight: 700;
    margin-bottom: 10px;
    text-transform: uppercase;
    color: #0A5C36;
}

.technical-text {
    font-size: 18px;
}

.sub-title {
    font-size: 24px;
    font-weight: 500;
    margin-bottom: 10px;
    text-transform: uppercase;
    color: #0A5C36;
}

.skill-group {
    margin-top: 30px;
    border-bottom: solid 2px gainsboro;
    padding-bottom: 30px;
}

.skills-wrapper {
    display: flex;
    flex-wrap: wrap;
}

@media (min-width: 576px) and (max-width: 767.98px) {
    .technical-text {
        font-size: 14px;
    }

    .technical-title {
        font-size: 22px;
        margin-bottom: 2px;
    }

    .sub-title {
        font-size: 22px;
        margin-bottom: 2px;
    }
}

@media (max-width: 575.98px) {
    .technical-text {
        font-size: 14px;
    }

    .technical-title {
        font-size: 22px;
        margin-bottom: 2px;
    }

    .sub-title {
        font-size: 22px;
        margin-bottom: 2px;
    }

    .skills-wrapper {
        height: 330px;
        overflow: scroll;
    }

    .skill-group {
        padding-bottom: 0px;
    }
}
</style>
  