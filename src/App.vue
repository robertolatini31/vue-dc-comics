<template>
  <div id="app">
   <SiteHeader />
   <SiteMain />
   <ServicesComponent />
   <SectionDcLists />
   <SiteFooter />
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import SiteHeader from '@/components/SiteHeader.vue'
import SiteMain from '@/components/SiteMain.vue'
import ServicesComponent from '@/components/ServicesComponent.vue'
import SectionDcLists from '@/components/SectionDcLists.vue'
import SiteFooter from '@/components/SiteFooter.vue'
export default {
  name: 'App',
  components: {
    // HelloWorld
    SiteHeader,
    SiteMain,
    ServicesComponent,
    SectionDcLists,
    SiteFooter,
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
  max-width: 100%;
  display: flex;
  flex-wrap: wrap;
  flex: 1 1 auto;
}

.col-2 {
  width: calc(100% / 12) * 2;
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
