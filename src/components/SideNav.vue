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
                {key:"1", title:"Lowkey Gamer", banner: require('../assets/gamer.jpg'), content:"I consider myself a lowkey gamer. Since my childhood days I do play console games and right now I do own a Nintendo Switch and I enjoy playing games like Pokemom, Legend of Zelda games (Breath of the Wild & Tears of the Kingdom), and various Super Mario games. I do also play MOBA games such as Pokemon Unite and league of legends / Wild Rift!"},
                {key:"2", title:"INTP Personality", banner: require('../assets/intp.jpg'), content:"The INTP personality type is known for being quiet, reserved, logical, and thoughtful. We are often described as introverted, intuitive, thinking, and perceiving. People with this personality type tend to be analytical and enjoy spending time alone, thinking about how things work, and coming up with solutions to different problems."},
                {key:"3", title:"Loves Dogs", banner: require('../assets/doglover.jpg'), content:"I love dogs, and indeed I believed that they are the man's bestfriend. We (My Family) do have a pet dog, and her name was Coco. I love her energy and the way she's excited to see me whenever I came home from work. Here's a fun fact: Studies have shown that interacting with dogs can lower blood pressure, heart rate, and stress hormones."},
                {key:"4", title:"Otaku at Heart", banner: require('../assets/otaku.jpg'), content:"I consider myself as an OTAKU, - a term used to describe someone who is passionate about Japanese pop culture, including anime, manga, video games, and technology. I grew up watching animes and reading manga, then as year passed by I found myself surrounded by friends with similar interest."},
                {key:"5", title:"Favorite color is RED", banner: require('../assets/red.jpg'), content:"I’ve lost count of how many things I owned that are color red. Whether it is bag, t-shirt, notebooks, and wallet! For me color red symbolizes my passion, my excitement and energy in my outlook on life."}
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
  