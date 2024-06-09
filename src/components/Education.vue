<template>
    <div class="education-holder">
        <p class="education-title">{{title}}</p>
        <p class="education-text">
            {{text}}
        </p>

        <div class="school-holder">
            <School></School>
            <School></School>
            <School></School>
        </div>
        
    </div>
</template>
  



<script>
  import School from './School.vue'
  export default {
    name: 'Education',
    components: {
        School,
    },
    props: ["title", "text"],
    data() {
        return {

        }
    }
  }
</script>
  



<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.education-holder {
    padding-bottom: 30px;
}

.education-title {
    font-size: 30px;
    font-weight: 700;
    margin-bottom: 10px;
    text-transform: uppercase;
    color: #0A5C36;
}

.education-text {
    font-size: 18px;
}

.school-holder {
    display: flex;
    margin-top: 20px;
 
}
</style>
  