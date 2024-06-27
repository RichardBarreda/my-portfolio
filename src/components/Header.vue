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
                        <a href="https://www.facebook.com/chardbarreda" class="header-link" target="_blank"><i class="bi bi-facebook"></i></a>
                    </div>
                    <div class="social-media">
                        <a href="https://www.linkedin.com/" class="header-link" target="_blank"><i class="bi bi-linkedin"></i></a>
                    </div>
                    <div class="social-media">
                        <a href="https://github.com/RichardBarreda" class="header-link" target="_blank"><i class="bi bi-github"></i></a>
                    </div>
                    <div class="social-media">
                        <a href="mailto:barredarichardmarck@gmail.com" class="header-link" target="_blank"><i class="bi bi-envelope-at-fill"></i></a>
                    </div>
                    <div class="social-media">
                        <a href="tel:09081452759" class="header-link" target="_blank"><i class="bi bi-telephone-fill"></i></a>
                    </div>
                </div>

                <button class="btn btn-outline-light mobile-menu" type="button" data-bs-toggle="offcanvas" data-bs-target="#staticBackdrop" aria-controls="staticBackdrop">
                    <i class="bi bi-list"></i>
                </button>

            </div>
        </div>
    </div>

    <div class="offcanvas offcanvas-start" data-bs-backdrop="static" tabindex="-1" id="staticBackdrop" aria-labelledby="staticBackdropLabel">
        <div class="offcanvas-header">
            <!-- <h5 class="offcanvas-title" id="staticBackdropLabel">Social Media</h5> -->
            <button type="button" class="btn-close" data-bs-dismiss="offcanvas" aria-label="Close"></button>
        </div>
        <div class="offcanvas-body">
            <div class="social-media-mobile">
                <div class="social-media-icon-holder">
                    <i class="bi bi-facebook mobile-bi-icon"></i>
                </div>
                <div class="social-media-text-holder">
                    <a class="media-text" href="https://www.facebook.com/chardbarreda" target="_blank">Facebook</a>
                </div>
            </div>

            <div class="social-media-mobile">
                <div class="social-media-icon-holder">
                    <i class="bi bi-linkedin mobile-bi-icon"></i>
                </div>
                <div class="social-media-text-holder">
                    <a class="media-text" href="https://www.linkedin.com/" target="_blank">Linkedin</a>
                </div>
            </div>

            <div class="social-media-mobile">
                <div class="social-media-icon-holder">
                    <i class="bi bi-github mobile-bi-icon"></i>
                </div>
                <div class="social-media-text-holder">
                    <a class="media-text" href="https://github.com/RichardBarreda" target="_blank">Github</a>
                </div>
            </div>

            <div class="social-media-mobile">
                <div class="social-media-icon-holder">
                    <i class="bi bi-envelope-at-fill mobile-bi-icon"></i>
                </div>
                <div class="social-media-text-holder">
                    <a class="media-text" href="mailto:barredarichardmarck@gmail.com" target="_blank">Email</a>
                </div>
            </div>

            <div class="social-media-mobile">
                <div class="social-media-icon-holder">
                    <i class="bi bi-telephone-fill mobile-bi-icon"></i>
                </div>
                <div class="social-media-text-holder">
                    <a class="media-text" href="tel:09081452759" target="_blank">Mobile</a>
                </div>
            </div>
        </div>
    </div>
</template>
  



<script>
import Activity from './SideActivity.vue'
import FactsAboutMe from './FactsAboutMe.vue'
import HelloWorld from './HelloWorld.vue';
  export default {
    name: 'Header',
    components: {
        Activity, FactsAboutMe
    },
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

.header-link {
    color: white;
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

.mobile-menu {
    display: none;
}

.offcanvas-body { 
    display: flex;
    align-items: center;
    flex-direction: column;
}

.social-media-mobile {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
    padding-bottom: 10px;
    padding-top: 10px;
}

.social-media-icon-holder {
    width: 45px;
    display: flex;
    justify-content: center;
    align-items: center;
}

.mobile-bi-icon {
    font-size: 30px;
}

.media-text {
    font-size: 20px;
    text-decoration: none;
    color: black;
}

@media (max-width: 575.98px) {
    .social-media-group {
        display: none;
    }

    .mobile-menu {
        display: block;
    }

    .title-text {
        font-size: 24px;
        letter-spacing: 0px;
    }
}

</style>
  