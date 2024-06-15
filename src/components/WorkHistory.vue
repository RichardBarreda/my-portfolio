<template>
    <div class="work-history">
      <Work :workid="workId1" :company="workCompany1" :date="workDate1" :website="workWeb1" :address="workAddress1" :position="workPosition1" :gallery="workGallery1">

        <template v-slot:bullet>
          <ul>
            <li class="bullet-items">Tincidunt vitae semper quis lectus nulla at. Nulla posuere sollicitudin aliquam ultrices sagittis orci a scelerisque.</li>
            <li class="bullet-items">Sagittis purus sit amet volutpat consequat mauris nunc. Eleifend mi in nulla posuere sollicitudin aliquam.</li>
            <li class="bullet-items">Viverra suspendisse potenti nullam ac tortor vitae purus faucibus. </li>
            <li class="bullet-items">Varius vel pharetra vel turpis nunc eget. Eu augue ut lectus arcu bibendum at varius vel pharetra.</li>
            <li class="bullet-items">Mus mauris vitae ultricies leo integer malesuada nunc. Lorem ipsum dolor sit amet consectetur adipiscing elit duis.</li>
            <li class="bullet-items">Orci dapibus ultrices in iaculis nunc sed. Consequat interdum varius sit amet mattis vulputate enim.</li>
            <li class="bullet-items">Sit amet risus nullam eget. Arcu dui vivamus arcu felis bibendum ut tristique et egestas. Enim facilisis gravida neque convallis a cras semper.</li>
            <li class="bullet-items">Volutpat sed cras ornare arcu. Arcu ac tortor dignissim convallis aenean. </li>
            <li class="bullet-items">Fringilla phasellus faucibus scelerisque eleifend donec pretium vulputate sapien nec. Dui id ornare arcu odio ut sem nulla.</li>
            <li class="bullet-items">Dapibus ultrices in iaculis nunc sed augue. Mi quis hendrerit dolor magna eget est lorem. Ultricies leo integer malesuada nunc vel risus commodo.</li>
          </ul>
          
        </template>

      </Work>

      <Work :workid="workId2" :company="workCompany2" :date="workDate2" :website="workWeb2" :address="workAddress2" :position="workPosition2" :gallery="workGallery2">

        <template v-slot:bullet>
          <ul>
            <li class="bullet-items">Tincidunt vitae semper quis lectus nulla at. Nulla posuere sollicitudin aliquam ultrices sagittis orci a scelerisque.</li>
            <li class="bullet-items">Sagittis purus sit amet volutpat consequat mauris nunc. Eleifend mi in nulla posuere sollicitudin aliquam.</li>
            <li class="bullet-items">Viverra suspendisse potenti nullam ac tortor vitae purus faucibus. </li>
            <li class="bullet-items">Varius vel pharetra vel turpis nunc eget. Eu augue ut lectus arcu bibendum at varius vel pharetra.</li>
            <li class="bullet-items">Mus mauris vitae ultricies leo integer malesuada nunc. Lorem ipsum dolor sit amet consectetur adipiscing elit duis.</li>
            <li class="bullet-items">Orci dapibus ultrices in iaculis nunc sed. Consequat interdum varius sit amet mattis vulputate enim.</li>
            <li class="bullet-items">Sit amet risus nullam eget. Arcu dui vivamus arcu felis bibendum ut tristique et egestas. Enim facilisis gravida neque convallis a cras semper.</li>
            <li class="bullet-items">Volutpat sed cras ornare arcu. Arcu ac tortor dignissim convallis aenean. </li>
            <li class="bullet-items">Fringilla phasellus faucibus scelerisque eleifend donec pretium vulputate sapien nec. Dui id ornare arcu odio ut sem nulla.</li>
            <li class="bullet-items">Dapibus ultrices in iaculis nunc sed augue. Mi quis hendrerit dolor magna eget est lorem. Ultricies leo integer malesuada nunc vel risus commodo.</li>
          </ul>
          
        </template>

      </Work>

      <Work :workid="workId3" :company="workCompany3" :date="workDate3" :website="workWeb3" :address="workAddress3" :position="workPosition3" :gallery="workGallery3">

        <template v-slot:bullet>
          <ul>
            <li class="bullet-items">Tincidunt vitae semper quis lectus nulla at. Nulla posuere sollicitudin aliquam ultrices sagittis orci a scelerisque.</li>
            <li class="bullet-items">Sagittis purus sit amet volutpat consequat mauris nunc. Eleifend mi in nulla posuere sollicitudin aliquam.</li>
            <li class="bullet-items">Viverra suspendisse potenti nullam ac tortor vitae purus faucibus. </li>
            <li class="bullet-items">Varius vel pharetra vel turpis nunc eget. Eu augue ut lectus arcu bibendum at varius vel pharetra.</li>
            <li class="bullet-items">Mus mauris vitae ultricies leo integer malesuada nunc. Lorem ipsum dolor sit amet consectetur adipiscing elit duis.</li>
            <li class="bullet-items">Orci dapibus ultrices in iaculis nunc sed. Consequat interdum varius sit amet mattis vulputate enim.</li>
            <li class="bullet-items">Sit amet risus nullam eget. Arcu dui vivamus arcu felis bibendum ut tristique et egestas. Enim facilisis gravida neque convallis a cras semper.</li>
            <li class="bullet-items">Volutpat sed cras ornare arcu. Arcu ac tortor dignissim convallis aenean. </li>
            <li class="bullet-items">Fringilla phasellus faucibus scelerisque eleifend donec pretium vulputate sapien nec. Dui id ornare arcu odio ut sem nulla.</li>
            <li class="bullet-items">Dapibus ultrices in iaculis nunc sed augue. Mi quis hendrerit dolor magna eget est lorem. Ultricies leo integer malesuada nunc vel risus commodo.</li>
          </ul>
          
        </template>

      </Work>
    </div>
</template>
  



<script>
  import Work from "./Work.vue"
  export default {
    name: 'WorkHistory',
    components: {
      Work
    },
    data() {
        return {
          workId1: "nanox",
          workCompany1: "Nanox Philippines Inc",
          workDate1: "October 2020 - Present",
          workWeb1: "https://nanoxphilippines.com/",
          workAddress1: "Clark Freeport, Mabalacat, Pampanga",
          workPosition1: "IT Support / Web Developer",
          workGallery1: [
            { key:"img1", location: require('../assets/nanox-img-1.jpg'), date: "October 16, 2022", caption: "Current IT Staff with OJT on a very ordinary day!"},
            { key:"img2", location: require('../assets/nanox-img-2.jpg'), date: "June 12, 2022", caption: "In vulputate ex et faucibus elementum. Nunc nisi libero, accumsan!"},
            { key:"img3", location: require('../assets/nanox-img-3.jpg'), date: "December 25, 2022", caption: "Suspendisse dolor neque, laoreet vel pulvinar a, rutrum non est."},
            { key:"img3", location: require('../assets/nanox-img-4.jpg'), date: "December 25, 2022", caption: "Suspendisse dolor neque, laoreet vel pulvinar a, rutrum non est."},
            { key:"img3", location: require('../assets/nanox-img-5.jpg'), date: "December 25, 2022", caption: "Suspendisse dolor neque, laoreet vel pulvinar a, rutrum non est."},
          ],

          workId2: "fullstack",
          workCompany2: "Fullstack HQ",
          workDate2: "April 2019 - March 2020",
          workWeb2: "https://fullstackhq.com/",
          workAddress2: "Sto. Rosario St. Angeles City, Pampanga",
          workPosition2: "Front End Developer",
          workGallery2: [
            { key:"img1", location: require('../assets/fullstack-img-1.jpg'), date: "September, 2019", caption: "Weekly Team Building Activity. All employees are divided into different teams to compete with various games."},
            { key:"img2", location: require('../assets/fullstack-img-2.jpg'), date: "October, 2019", caption: "Monthly Birthday Celebration! Also TGIF because we usually schedule this kind of party every last friday of the month!"},
            { key:"img3", location: require('../assets/fullstack-img-3.jpg'), date: "December 22, 2019", caption: "Fullstack HQ Year-End Thanksgiving Party 2019! Celebrating with lots of foods, games, prizes and gifts for everyone!"},
            { key:"img4", location: require('../assets/fullstack-img-4.jpg'), date: "August 16-17, 2019", caption: "FSHQ team celebrated the company's 4th year at Villa de Venancia last 2019. Definitely one for the books!"},
            { key:"img5", location: require('../assets/fullstack-img-5.jpg'), date: "February 27, 2020", caption: "Pizza, spaghetti, and drinks are in! Here we are Celebrating small wins with our project team."},
          ],

          workId3: "mvp",
          workCompany3: "MVP Asia Pacific Inc.",
          workDate3: "November 2018 - March 2019",
          workWeb3: "https://www.offshoremvp.com/",
          workAddress3: "Philexcel Business Park Clark Freeport, Mabalacat, Pampanga",
          workPosition3: "OJT - Front End Developer",
          workGallery3: [
            { key:"img1", location: require('../assets/mvp-img-1.jpg'), date: "October 16, 2022", caption: "Current IT Staff with OJT on a very ordinary day!"},
            { key:"img2", location: require('../assets/mvp-img-2.jpg'), date: "June 12, 2022", caption: "In vulputate ex et faucibus elementum. Nunc nisi libero, accumsan!"},
            { key:"img3", location: require('../assets/mvp-img-3.jpg'), date: "December 25, 2022", caption: "Suspendisse dolor neque, laoreet vel pulvinar a, rutrum non est."},
          ],
        }
    }
  }
</script>
  



<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.bullet-items {
  font-size: 17px;
  color: rgb(14, 14, 14);
  list-style-type:square;
}
</style>
  