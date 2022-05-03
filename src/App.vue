<template>
  <div id="app">
   <SiteHeader />
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import SiteHeader from './components/SiteHeader.vue'

export default {
  name: 'App',
  components: {
    // HelloWorld
    SiteHeader,
    
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}

* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

img {
  max-width: 100%;
}

.container {
  margin: auto;
  max-width: 1440px;
}

.row {
  width: 100%;
  display: flex;
  flex-wrap: wrap;
}

.col-4 {
  width: calc(100% / 12) * 4;
}

.col-6 {
    width: calc(100% / 2);
}

.col-8 {
  width: calc(100% / 12) * 8;
}

</style>
