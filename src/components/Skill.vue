<template>
    <div class="skills-holder">
      <div class="icon-holder">
        <img :src="icon" class="img-fluid img-skills"/>
      </div>
      <div class="details-holder">
        <p class="skill-name">{{name}}</p>
        <div class="confidence-scale">
          <div class="confidence-level" :style="'width:'+level"></div>
        </div>
        <p class="confidence-label">Confidence Level: {{level}}</p>
      </div>
    </div>
</template>
  



<script>
  export default {
    name: 'Skills',
    props: ["name", "icon", "level"],
    data() {
        return {

        }
    }
  }
</script>
  



<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.skills-holder {
    width: 31%;
    max-width: 100%;
    margin-right: 15px;
    margin-top: 20px;

    display: flex;

    background-color: #ededed;
    height: 80px;

    box-shadow: 0 1px 3px rgba(0, 0, 0, 0.12), 0 1px 2px rgba(0, 0, 0, 0.24);
    transition: all 0.3s cubic-bezier(0.25, 0.8, 0.25, 1);
}

.skills-holder:hover {
  transition: all 0.3s cubic-bezier(0.25, 0.8, 0.25, 1);
  box-shadow: 0 14px 28px rgba(0, 0, 0, 0.25), 0 10px 10px rgba(0, 0, 0, 0.22);
}

.icon-holder {
    width: 30%;
    background-color: white;
    max-width: 100%;
    height: 100%;
    padding: 15px;
}

.img-fluid {
  max-width: 100%;
  width: 100%;
  height: 100%;
  object-fit: contain;
}

.details-holder {
  padding: 10px;
  width: 70%;
}

.skill-name {
  font-size: 18px;
  font-weight: 500;
}

.confidence-scale{
  height: 15px;
  width: 100%;
  background-color: #cfcfcf;
  border: solid 1px #c1c1c1;
  position: relative;
}

.confidence-level {
  height: 14px;
  background-color: #399968;
  border: solid 1px #399968;
}

.confidence-label {
  font-size: 11px;
  text-transform: uppercase;
  color: #626262;
}

.test {
  font-size: 20px;
}
</style>
  