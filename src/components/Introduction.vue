<template>
    <div class="introduction-holder">
        <p class="introduction-title">{{title}}</p>
        <p class="introduction-text">
            {{text}}
        </p>

        
    </div>
</template>
  



<script>
  export default {
    name: 'Introduction',
    props: ["title", "text"],
    data() {
        return {

        }
    }
  }
</script>
  



<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.introduction-holder {
    padding-bottom: 30px;
}

.introduction-title {
    font-size: 30px;
    font-weight: 700;
    margin-bottom: 10px;
    text-transform: uppercase;
    color: #0A5C36;
}

.introduction-text {
    font-size: 18px;
}
</style>
  