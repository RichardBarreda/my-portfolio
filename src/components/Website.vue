<template>
    <div class="website-holder" :style="'background-color:'+theme">
        <div class="website-banner">
            <img :src="image" class="img-fluid" />
        </div>
        <div class="website-information" :style="'background-color:'+theme">
            <a :href="link" target="_blank" class="website-title">{{name}}</a>
            <div class="website-language">
                <div class="lang-holder" v-for="lang in language" :key="lang">{{lang}}</div>
            </div>
            <p class="website-description">
                {{description}}
            </p>
        </div>
    </div>
</template>
  



<script>
  export default {
    name: 'Website',
    props: ["name", "image", "link", "language", "description", "theme"],
    data() {
        return {

        }
    }
  }
</script>
  



<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.website-holder {
    width: 31%;
    max-width: 100%;
    margin-right: 15px;
    margin-top: 20px;

    box-shadow: 0 1px 3px rgba(0, 0, 0, 0.12), 0 1px 2px rgba(0, 0, 0, 0.24);
    transition: all 0.3s cubic-bezier(0.25, 0.8, 0.25, 1);
}

.website-holder:hover {
    transition: all 0.3s cubic-bezier(0.25, 0.8, 0.25, 1);
    box-shadow: 0 14px 28px rgba(0, 0, 0, 0.25), 0 10px 10px rgba(0, 0, 0, 0.22);
}

.website-banner {
    height: 135px;
}

.img-fluid {
    max-width: 100%;
    height: 100%;
    width: 100%;
    object-fit: cover;
}

.website-information {
    color: white;
    padding: 10px 12px;
    text-align: center;
}

.website-title {
    font-size: 18px;
    font-weight: 500;
    text-decoration: none;
    color: white;
}

.website-title:hover {
    text-decoration: underline;
}

.website-language {
    display: flex;
    justify-content: center;
    align-items: center;
    margin-bottom: 15px;
    flex-wrap: wrap;
}

.lang-holder {
    font-size: 12px;
    background-color: #ffffff4a;
    margin-right: 5px;
    padding: 0px 5px;
    border-radius: 10px;
    margin-top: 5px;
}

.website-description {
    font-size: 14px;
    line-height: 19px;
}

@media (min-width: 992px) and (max-width: 1199.98px) {
  .website-holder {
    width: 45%;
  }
}

@media (min-width: 768px) and (max-width: 991.98px) {
    .website-holder {
        width: 45%;
    }
}

@media (min-width: 576px) and (max-width: 767.98px) {
    .website-holder {
        width: 100%;
    }
}

@media (max-width: 575.98px) {
    .website-holder {
        width: 100%;
    }
}
</style>
  