<template>
    <div class="activity-holder">
        <div class="cover-advice">
          <div class="banner-wrapper">
            <p class="section-title">TRY THIS!</p>
            <img src="../assets/advice.jpg" class="img-wrapper"/>
          </div>
          <div class="text-wrapper">
            <button type="button" @click="setAdvice" class="btn btn-primary btn-advice" data-bs-toggle="modal" data-bs-target="#adviceModal"> <i class="bi bi-dice-3"></i> Random Advice</button>
          </div>
        </div>
    </div>

    <!-- Modal -->
    <div class="modal fade" id="adviceModal" tabindex="-1" aria-labelledby="adviceModalLabel" aria-hidden="true">
      <div class="modal-dialog modal-dialog-centered custom-modal-dialog">
        <div class="modal-content">
          
          <div class="custom-modal-body">
            <div class="background-overlay"></div>
            <img :src="adviceCover" class="advice-cover-wrapper"/>
            <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
            <div class="advice-content">
              <p class="advice-title">{{adviceTitle}}</p>
              <p class="advice-text">{{adviceText}}</p>
            </div>
          </div>
          
        </div>
      </div>
    </div>

</template>
  



<script>
  export default {
    name: 'Activity',
    data() {
        return {
          randomNumber: "",
          adviceCover: "",
          adviceTitle: "",
          adviceText: "",
          adviceTotal: "",
          advice:[
                {key:"1", cover: require('../assets/advice-1.jpg'), title:"Go Exploring!", text:"Explore ideas, places, and opinions. The inside of the echo chamber is where all the boring people hang out."},
                {key:"2", cover: require('../assets/advice-2.jpg'), title:"Do not wait until tomorrow!", text:"Say, do, or make it now. Go where you need to be. Do not wait to be invited places. Host your own parties. Do not sit by the phone. Pick it up. Spread the word. Press the button. Buy the ticket and enjoy the show."},
                {key:"3", cover: require('../assets/advice-3.jpg'), title:"State the obvious!", text:"What's known to you is often a mystery to others. Your old fact is someone else's new lesson. Your simple task is someone else's imposible chore. Your mind is full of treasures that no one else has seen. Pass them on. An idea shared is not diminished: It's multiplied."},
                {key:"4", cover: require('../assets/advice-4.jpg'), title:"Give yourself some credit!", text:"You deserve a chance. You deserve to have fun. You deserve to be happy. You got abilities & curiosities & things to offer. So go on, jump in there. Not only is there room for you, there's a need for you. Really."},
                {key:"5", cover: require('../assets/advice-5.jpg'), title:"Embrace your weirdness!", text:"No one is normal. Everyone has quirks and insights unique to themselves. Don't hide these things, they are what makes you interesting."},
                {key:"6", cover: require('../assets/advice-6.jpg'), title:"Play Devil's Advocate!", text:"Do the opposite of expected. Defend the guilty. Question the pure. See which facts are opinions and which opinions are facts. There are many sides to every story, and they all need to be told."},
                {key:"7", cover: require('../assets/advice-7.jpg'), title:"Childlike Not Childish", text:"Look with open eyes. Remember how amazing the world was before you learned to be cynical. See the neat things. The messy things. The funny things. Less crankiness. More Marveling"},
                {key:"8", cover: require('../assets/advice-8.jpg'), title:"Why Not?", text:"Afraid to fail? Afraid to fail and that other people might find out about it? So what if you fail? Really: So what if you fail? Would that really be so bad?"},
                {key:"9", cover: require('../assets/advice-9.jpg'), title:"Try Again!", text:"Give extra chances, ESPECIALLY to yourself. If you're not dead, you can still change things."},
                {key:"10", cover: require('../assets/advice-10.jpg'), title:"Remain a Student", text:"Sign up to learn things. Philosophy, archery, accounting, painting, driving, fire eating -anything you admit you do not understand. You never know when you'll need a random skill."},
            ]
        }
    },
    methods: {
      setAdvice() {
        this.adviceTotal = this.advice.length;
        this.randomNumber = Math.floor(Math.random() * this.adviceTotal);
        this.adviceCover = this.advice[this.randomNumber].cover;
        this.adviceTitle = this.advice[this.randomNumber].title;
        this.adviceText = this.advice[this.randomNumber].text;
      }
    },
  }
</script>
  



<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.activity-holder {
    width: 100%;
    max-width: 100%;
    border-radius: 3px;
    background-color: #c1c1c1;
    margin-bottom: 30px;

    box-shadow: 0 3px 6px rgba(0, 0, 0, 0.16), 0 3px 6px rgba(0, 0, 0, 0.23);
}

.cover-advice {

}

.banner-wrapper {
  position: relative;
  padding: 15px;
  background-color: whitesmoke;
}

.section-title {
    position: absolute;
    font-size: 14px;
    font-weight: 500;
    color: black;
    background-color: #ffffffa8;
    top: 25px;
    left: 25px;
    padding: 3px 10px;
    z-index: 1;
}

.img-wrapper {
  height: 200px;
  width: 100%;
  max-width: 100%;
  object-fit: cover;
  border-radius: 10px;
}

.advice-cover-wrapper {
  height: 400px;
  width: 100%;
  max-width: 100%;
  object-fit: cover;
}

.text-wrapper {
  padding: 0px 0px 15px 0px;
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: whitesmoke;
}

.btn-advice {
  background: -webkit-linear-gradient(45deg, #6d78e1, #68d593 95%);
  color: white;
  font-size: 14px;
  font-weight: 500;
  text-transform: uppercase;
}

.bi-dice-3 {
  margin-right: 5px;
}

.btn-advice:hover {
  color: #0014FF;
  background: white;
}


.custom-modal-dialog {
  width: 100%;
  max-width: 800px;
}

.custom-modal-body {
  position: relative;
}

.background-overlay {
  position: absolute;
  width: 100%;
  height: 100%;
  top: 0;
  left: 0;
  background-color: #313131;
  opacity: 0.5;
  z-index: 0;
}

.advice-content {
  position: absolute;
  bottom: 0;
  z-index: 1;
  padding: 40px 30px;
}

.advice-title {
  width: fit-content;
  background-color: #f5f5f5b8;
  padding: 3px 10px;
  font-size: 22px;
  font-weight: 500;
  color: black;
  text-transform: uppercase;
  margin-bottom: 15px;
}

.advice-text {
  color: whitesmoke;
  font-weight: 500;
  font-size: 20px;
  text-shadow: 1px 1px black;
}

.btn-close {
  position: absolute;
  z-index: 1;
  top: 10px;
  right: 10px;
  background-color: whitesmoke;
  padding: 8px;
}


@media (max-width: 575.98px) {
  .custom-modal-dialog {
    width: auto;
  }

  .background-overlay {
      border: solid 3px white;
  }
  
  .advice-text {
    font-size: 16px;
    line-height: 20px;
  }

  .advice-title {
    font-size: 16px;
  }
}

</style>
  