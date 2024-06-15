<template>
    <div class="banner-holder">
        <div class="background-overlay"></div>
        <div class="profile-container">
            <div class="img-container">
                <img :src="avatarIcon" class="img-fluid img-avatar"/>
            </div>
            <div class="info-container">
                <p class="txt-greetings">{{greetings}}</p>
                <p class="txt-name">I'M <span class="my-name">{{name}}</span></p>
                <p class="txt-title">{{jobTitle}}</p>
            </div>
        </div>
        <div class="links-container">
            <button type="button" class="btn btn-outline-light profile-btn">{{btnDownload}}</button>
            <button type="button" class="btn btn-light profile-btn" data-bs-toggle="modal" data-bs-target="#exampleModal">{{btnMessage}}</button>
        </div>
    </div>

    <MessageMe></MessageMe>
</template>
  



<script>
  import MessageMe from "./MessageMe.vue"
  export default {
    name: 'Banner',
    components: {
        MessageMe
    },
    data() {
        return {
            avatarIcon: require('../assets/me-real.jpg'),

            greetings: "Hello There!",
            name: "RICHARD",
            jobTitle: "IT SPECIALIST / WEB DEVELOPER",

            btnDownload: "DOWNLOAD CV",
            btnMessage: "MESSAGE ME",
        }
    }
  }
</script>
  



<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.banner-holder {
    width: 100%;
    max-width: 100%;
    height: 350px;
    border-radius: 10px;

    background-image: url(../assets/banner.jpg);
    background-position: bottom;
    background-size: cover;
    position: relative;

    display: flex;
    align-items: flex-end;
    padding: 30px;
    justify-content: space-between;

    box-shadow: 0 3px 6px rgba(0, 0, 0, 0.16), 0 3px 6px rgba(0, 0, 0, 0.23);
}

.background-overlay {
    position: absolute;
    width: 100%;
    height: 100%;
    top: 0;
    left: 0;
    background-color: #575757;
    opacity: 0.7;
    z-index: 0;
    border-radius: 10px;
}

.links-container {
    z-index: 0;
    display: flex; 
    flex-direction: column;
}

.profile-container {
    display: flex;
    justify-content: center;
    align-items: center;
    z-index: 1;
}

.img-avatar {
    width: 160px;
    border-radius: 100px;
    object-fit: cover;
    height: 160px;

    box-shadow: 0 14px 28px rgba(0,0,0,0.25), 0 10px 10px rgba(0,0,0,0.22);
}

.info-container {
    margin-left: 30px;
    
}

.txt-greetings {
    font-size: 20px;
    font-weight: 500;
    text-transform: uppercase;
    line-height: 20px;
    color: white;
    text-shadow: 2px 2px 4px #000000;
}

.txt-name {
    font-size: 50px;
    font-weight: 500;
    text-transform: uppercase;
    line-height: 60px;
    color: white;
    text-shadow: 2px 2px 4px #000000;
}

.my-name {
    background: -webkit-linear-gradient(45deg, #42A5F5, #00ff95 70%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    margin: 0;
    text-shadow: none;
    font-weight: 700;

    filter: drop-shadow(2px 2px #333);
}

.txt-title {
    font-size: 15px;
    background-color: #004D40;
    color: white;
    padding: 0px 15px;
    width: fit-content;
}

.profile-btn {
    margin-top: 10px;
    font-size: 14px;
    font-weight: 500;
}

.profile-btn:hover {
    background: -webkit-linear-gradient(45deg, #42A5F5, #00ff95 70%);
    color: black;
    border-color: #004D40;
}

</style>
  