<template>
    <div class="activity-holder">
        <div class="cover-advice">
          <div class="banner-wrapper">
            <img src="../assets/advice.jpg" class="img-wrapper"/>
          </div>
          <div class="text-wrapper">
            <button type="button" class="btn btn-primary btn-advice"> <i class="bi bi-dice-3"></i> Random Advice</button>
          </div>
        </div>
    </div>
</template>
  



<script>
  export default {
    name: 'Activity',
    data() {
        return {
          advice:[
                {key:"1", text:"Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Scelerisque eleifend donec pretium vulputate."},
                {key:"2", text:"Commodo viverra maecenas accumsan lacus vel facilisis volutpat. Massa id neque aliquam vestibulum morbi. Scelerisque in dictum non consectetur a."},
                {key:"3", text:"Diam in arcu cursus euismod quis viverra. Diam phasellus vestibulum lorem sed risus ultricies tristique nulla aliquet. In est ante in nibh mauris cursus mattis."},
                {key:"4", text:"Pellentesque elit ullamcorper dignissim cras. Imperdiet massa tincidunt nunc pulvinar sapien et. Sodales neque sodales ut etiam sit amet nisl. Eu volutpat."},
                {key:"5", text:"Massa tempor nec feugiat nisl pretium fusce id. Auctor elit sed vulputate mi sit amet mauris commodo."},
            ]
        }
    }
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
  
}

.img-wrapper {
  height: 200px;
  width: 100%;
  max-width: 100%;
  object-fit: cover;
}

.text-wrapper {
  height: 100px;
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

</style>
  