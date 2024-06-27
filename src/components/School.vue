<template>
    <div class="school-holder">
        <div class="logo-holder">
          <img class="img-fluid" :src="hauLogo">
        </div>
        <div class="details-holder">
          <p class="education-title">BACHELOR OF SCIENCE IN COMPUTER SCIENCE</p>
          <p class="school-name">Holy Angel University</p>
          <p class="school-date">June 2015 - May 2019</p>
        </div>
    </div>

    <div class="school-holder">
        <div class="logo-holder">
          <img class="img-fluid" :src="hauLogo">
        </div>
        <div class="details-holder">
          <p class="education-title">SECONDARY EDUCATION</p>
          <p class="school-name">Holy Angel University</p>
          <p class="school-date">June 2011 - March 2015</p>
        </div>
    </div>

    <div class="school-holder">
        <div class="logo-holder">
          <img class="img-fluid" :src="vtesLogo">
        </div>
        <div class="details-holder">
          <p class="education-title">PRIMARY EDUCATION</p>
          <p class="school-name">Villa Teodora Elementary School</p>
          <p class="school-date">June 2005  - May 2011</p>
        </div>
    </div>
</template>
  



<script>
  export default {
    name: 'School',
    data() {
        return {
          hauLogo: require('../assets/hau.jpg'),
          vtesLogo: require('../assets/vtes.png'),
        }
    }
  }
</script>
  



<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.school-holder {
  margin-top: 20px;
  display: flex;
}

.logo-holder {
  width: 100%;
  max-width: 100px;
}

.education-title {
  font-size: 18px;
  font-weight: 500;
}

.details-holder {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: flex-start;
    padding-left: 10px;
}

.school-name {
  font-size: 18px;
  color: black;
}

.school-date {
  font-size: 16px;
  color: #5f5f5f;
}
</style>
  