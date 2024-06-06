<template>
  <Header></Header>
  <Body></Body>
</template>

<script>
import Header from './components/Header.vue'
import Body from './components/Body.vue'


export default {
  name: 'App',
  components: {
    Header, Body
  }
}
</script>

<style>

.custom-container {
  width: 100%;
  max-width: 100%;
  padding: 0px 30px;
}

p {
  padding: 0px;
  margin: 0px
}

</style>
