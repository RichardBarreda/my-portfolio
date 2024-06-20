<template>
    <div class="content-holder">
        <Banner></Banner>
        <Accordion></Accordion>
    </div>
</template>
  



<script>
import Banner from './Banner.vue'
import Accordion from './Accordion.vue'

  export default {
    name: 'Content',
    components: {
        Banner, Accordion
    },
    data() {
        return {

        }
    }
  }
</script>
  



<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.content-holder {
    width: 70%;
    max-width: 100%;
    
    padding-right: 15px;
}

@media (max-width: 991.98px) {
    .content-holder {
        width: 100%;
        padding-right: 0px;
    }
}
</style>
  