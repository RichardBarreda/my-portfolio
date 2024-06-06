<template>
    <div class="work-holder">
        <div class="title-wrapper">
            <p class="work-company">{{company}}</p>
            <p class="work-date"> <i class="bi bi-calendar work-icon"></i> {{date}}</p>
            <p class="work-position"> <i class="bi bi-person-workspace work-icon"></i> {{position}}</p>
        </div>
        <slot name="bullet"></slot>
    </div>
</template>
  



<script>
  export default {
    name: 'Work',
    props: ["company", "date", "position"],
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
}

.work-company {
    font-size: 30px;
    font-weight: 700;
    margin-bottom: -5px;
    text-transform: uppercase;
    color: #0A5C36;
}

.work-date {
    font-size: 18px;
}

.work-position {
    font-size: 18px;
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

</style>
  