<template>
    <div class="education-holder">
        <p class="education-title">{{title}}</p>

        <div class="school-holder">
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
    flex-direction: column;
}

@media (min-width: 576px) and (max-width: 767.98px) {
    .education-text {
        font-size: 14px;
    }

    .education-title {
        font-size: 22px;
        margin-bottom: 2px;
    }
}

@media (max-width: 575.98px) {
    .education-text {
        font-size: 14px;
    }

    .education-title {
        font-size: 22px;
        margin-bottom: 2px;
    }
}
</style>
  