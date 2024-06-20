<template>
    <div class="work-holder">
        <div class="title-wrapper">
            <div class="company-group">
                <p class="work-company">{{company}}</p>
                <button type="button" class="btn btn-outline-secondary" data-bs-toggle="modal" :data-bs-target="'#galleryModal'+workid"><i class="bi bi-card-image"></i></button>
            </div>
            
            <p class="work-position">{{position}}</p>
            <p class="work-info"> <i class="bi bi-calendar work-icon"></i> {{date}}</p>
            <p class="work-info"> <i class="bi bi-geo-alt-fill work-icon"></i> {{address}}</p>
            <a class="work-info work-link" :href="website" target="_blank"> <i class="bi bi-link-45deg work-icon"></i> {{website}}</a>
        </div>
        <slot name="bullet"></slot>
    </div>

    <div class="modal fade" :id="'galleryModal'+workid" tabindex="-1" aria-labelledby="galleryModal" aria-hidden="true">
        <div class="modal-dialog">
            <div class="modal-content">
                <div class="gallery-container" >
                    <div :id="'carousel'+workid" class="carousel slide">

                        <div class="head-holder">
                            <div class="company-holder">
                                <p class="gallery-company">{{company}}</p>
                                <p class="gallery-date"> <i class="bi bi-calendar gallery-icon-date"></i>{{date}}</p>
                            </div>  
    
                            <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                        </div>
                        
                        <div class="carousel-inner">
                            <div class="carousel-item" :class="{ active: picture.key=='img1' }" v-for="picture in gallery" :key="picture.key">
                                <p class="gallery-description">{{picture.caption}}</p>
                                <div class="gallery-border">
                                    <img :src="picture.location" class="d-block w-100 img-fluid" alt="...">
                                    <p class="date-float">{{picture.date}}</p>
                                </div>
                                
                            </div>
                        </div>

                        <div class="footer-holder">
                            <div class="footer-group footer-group-emote">
                                <div class="gallery-emote"> <i class="bi bi-hand-thumbs-up-fill"></i> </div>
                                <div class="gallery-emote"> <i class="bi bi-heart-fill"></i> </div>
                                <div class="gallery-emote"> <i class="bi bi-emoji-sunglasses-fill"></i> </div>
                                <div class="gallery-emote"> <i class="bi bi-award-fill"></i> </div>
                                <div class="gallery-emote"> <i class="bi bi-rocket-takeoff-fill"></i> </div>
                            </div>
                            <div class="footer-group">
                                <button type="button" class="btn btn-success gallery-button" :data-bs-target="'#carousel'+workid" data-bs-slide="prev"><i class="bi bi-caret-left-fill"></i> PREVIOUS</button>
                                <button type="button" class="btn btn-success gallery-button" :data-bs-target="'#carousel'+workid" data-bs-slide="next">NEXT <i class="bi bi-caret-right-fill"></i></button>
                            </div>
                            
                        </div>

                    </div>
                </div>
            </div>
        </div>
    </div> 
</template>
  



<script>
  export default {
    name: 'Work',
    props: ["workid", "company", "date", "position", "website", "address", "gallery"],
    data() {
        return {

        }
    }
  }
</script>
  



<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.work-holder {
    padding-bottom: 30px;
    margin-bottom: 30px;
    border-bottom: solid 2px lightgray;
}

.work-company {
    font-size: 30px;
    font-weight: 700;
    margin-bottom: -5px;
    text-transform: uppercase;
    color: #0A5C36;
}

.head-holder {
    display: flex;
    justify-content: space-between;
}

.company-group {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.gallery-container {
    padding: 20px;
}

.gallery-company {
    font-size: 22px;
    color: black;
    font-weight: 700;
    text-transform: uppercase;
}

.gallery-date {
    font-size: 15px;
    color: gray;
}

.gallery-icon-date {
    margin-right: 3px;
}

.gallery-border {
    border: solid 2px #198754;
    position: relative;
}

.img-fluid {
    height: 300px;
    width: 100%;
    max-width: 100%;
    object-fit: cover;
}

.date-float {
    position: absolute;
    top: 10px;
    background-color: white;
    color: black;
    left: 10px;
    padding: 0px 5px;
    font-size: 14px;
    opacity: .5;
    text-transform: uppercase;

}

.gallery-description {
    margin-top: 20px;
    font-size: 18px;
    color: black;
    text-decoration: none;

    display: none;
}

.footer-holder {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding-top: 15px;
}

.footer-group {
    display: flex;
    justify-content: center;
    align-items: center;
}

.gallery-emote {
    font-size: 25px;
    color: #198754;
    margin-right: 15px;
}

.gallery-button {
    margin-left: 10px;
    width: 120px;
}

.modal-dialog {
    width: 600px;
    max-width: 100%;

    box-shadow: 0 3px 6px rgba(0, 0, 0, 0.16), 0 3px 6px rgba(0, 0, 0, 0.23);
}

.modal-content {
    border-radius: 0px;
}

.work-info {
    font-size: 18px;
    color: black;
    text-decoration: none;
}

.work-position {
    font-size: 17px;
    color: white;
    text-decoration: none;
    background-color: #004D40;
    width: fit-content;
    padding: 0px 10px;
    margin-bottom: 10px;
    border-radius: 10px;
}

.work-link:hover {
    color: blue;
}

.work-text {
    font-size: 18px;
}

.title-wrapper {
    padding-bottom: 30px;
}

.work-icon {
    margin-right: 3px;
    font-weight: 500;
    font-size: 18px;
}

@media (min-width: 576px) and (max-width: 767.98px) {
  .work-info {
    font-size: 15px;
    line-height: 20px;
  }

  .work-position {
    font-size: 15px;
    margin-bottom: 5px;
  }

  .work-company {
    font-size: 24px;
  }
}

@media (max-width: 575.98px) {
    .work-info {
    font-size: 15px;
    line-height: 20px;

    text-indent: -13px;
    margin-left: 25px;
  }

  .work-position {
    font-size: 15px;
    margin-bottom: 10px;
  }

  .work-link {
    margin-left: 10px;
  }

  .work-company {
    font-size: 20px;
  }

  .modal-dialog {
    width: auto;
  }

  .img-fluid {
    height: 230px;
    object-position: right;
  }

  .footer-group-emote {
    display: none;
  }

  .footer-group {
    width: 100%;
  }

  .gallery-button {
        margin-left: 5px;
        width: 100%;
        margin-right: 5px;
    }
}

</style>
  