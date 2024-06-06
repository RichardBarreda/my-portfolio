<template>
    <div class="side-nav-holder">
        <Activity></Activity>
        <Activity></Activity>
    </div>
</template>
  



<script>
import Activity from './SideActivity.vue'
  export default {
    name: 'SideNav',
    components: {
        Activity,
    },
    data() {
        return {

        }
    }
  }
</script>
  



<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.side-nav-holder {
    width: 30%;
    max-width: 100%;
    
    padding-left: 15px;
}
</style>
  