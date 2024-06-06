<template>
    <div class="article-holder">
        <p class="article-title">{{title}}</p>
        <p class="article-text">
            {{text}}
        </p>

        
    </div>
</template>
  



<script>
  export default {
    name: 'Article',
    props: ["title", "text"],
    data() {
        return {

        }
    }
  }
</script>
  



<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.article-holder {
    padding-bottom: 30px;
}

.article-title {
    font-size: 30px;
    font-weight: 500;
}

.article-text {
    font-size: 18px;
}
</style>
  