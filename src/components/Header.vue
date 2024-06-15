<template>
    <div class="header-holder">
        <div class="custom-container">
            <div class="content-holder">
                <div class="portfolio-title">
                    <i class="bi bi-journal-album head-icon"></i>
                    <p class="title-text">MY PORTFOLIO</p>
                </div>
                <div class="social-media-group">
                    <div class="social-media">
                        <i class="bi bi-facebook"></i>
                    </div>
                    <div class="social-media">
                        <i class="bi bi-linkedin"></i>
                    </div>
                    <div class="social-media">
                        <i class="bi bi-github"></i>
                    </div>
                    <div class="social-media">
                        <i class="bi bi-envelope-at-fill"></i>
                    </div>
                    <div class="social-media">
                        <i class="bi bi-telephone-fill"></i>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
  



<script>
import HelloWorld from './HelloWorld.vue';
  export default {
    name: 'Header',
    data() {
        return {

        }
    }
  }
</script>
  


<!-- background-color: #14452F; -->
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.header-holder {
    height: 65px;
    width: 100%;
    max-width: 100%;
    background: -webkit-linear-gradient(45deg, #0A5C36, #18392B 70%);
}

.custom-container {
    height: 100%;
}

.content-holder {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 100%;
}

.portfolio-title {
    display: flex;
    justify-content: center;
    align-items: center;
}

.head-icon {
    font-size: 28px;
    color: white;
    font-weight: 700;
    margin-right: 10px;
}

.title-text {
    font-size: 28px;
    color: white;
    font-weight: 700;
    font-family: monospace;
}

.social-media-group {
    display: flex;
    color: white;
    font-size: 25px;
}

.social-media {
    padding: 0px 10px;
}

.social-media:hover {
    cursor: pointer;
    opacity: .5;
}

</style>
  