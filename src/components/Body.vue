<template>
    <div class="body-holder">
        <div class="custom-container">
            <div class="body-wrapper">
                <Content></Content>
                <SideNav></SideNav>
            </div>
        </div>
    </div>
</template>
  



<script>
import Content from './Content.vue';
import SideNav from './SideNav.vue';
  export default {
    name: 'Body',
    components: {
        Content, SideNav
    },
    data() {
        return {

        }
    }
  }
</script>
  



<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.body-holder {
    padding: 30px 0px;
    width: 100%;
    max-width: 100%;
    background-color: #e5e3e3;
}

.body-wrapper {
    display: flex;
}

@media (max-width: 991.98px) { 
    .body-wrapper {
        flex-direction: column;
    }
}
</style>
  