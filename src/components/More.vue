<template>
    <div class="more-holder">
      <p class="more-title">Additional</p>
        <SideNav></SideNav>
    </div>
</template>
  



<script>
 import SideNav from './SideNav.vue';
  export default {
    name: 'More',
    components: {
        SideNav
    },
    data() {
        return {
         
        }
    }
  }
</script>
  



<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.more-holder .side-nav-holder {
    display: block;
    width: 100%;
    padding-left: 0px;
    margin-top: 20px;
}

.more-title {
  font-size: 30px;
  font-weight: 700;
  margin-bottom: 10px;
  text-transform: uppercase;
  color: #0A5C36;
}

@media (max-width: 575.98px) {
  .more-text {
    font-size: 14px;
  }

  .more-title {
        font-size: 22px;
        margin-bottom: 2px;
    }  
}
</style>
  