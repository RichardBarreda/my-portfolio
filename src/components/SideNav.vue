<template>
    <div class="side-nav-holder">
        <FactsAboutMe :content="facts"></FactsAboutMe>
        <Activity></Activity>
    </div>
</template>
  



<script>
import Activity from './SideActivity.vue'
import FactsAboutMe from './FactsAboutMe.vue'

  export default {
    name: 'SideNav',
    components: {
        Activity, FactsAboutMe
    },
    data() {
        return {
            facts:[
                {key:"1", title:"Lowkey Gamer", banner: require('../assets/gamer.jpg'), content:"Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur."},
                {key:"2", title:"INTP Personality", banner: require('../assets/intp.jpg'), content:"Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur."},
                {key:"3", title:"Loves Dogs", banner: require('../assets/doglover.jpg'), content:"Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur."},
                {key:"4", title:"Otaku at Heart", banner: require('../assets/otaku.jpg'), content:"Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur."},
                {key:"5", title:"Favorite color is RED", banner: require('../assets/red.jpg'), content:"Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur."}
            ],
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

@media (min-width: 992px) and (max-width: 1199.98px) {
    
}

@media (min-width: 768px) and (max-width: 991.98px) {
    
}

@media (max-width: 991.98px) { 
    .side-nav-holder {
        display: none;
    }
}

@media (min-width: 576px) and (max-width: 767.98px) {

}

@media (max-width: 575.98px) {

}


</style>
  