<template>
  <div id="app">
    <Header/>
    <main>
      <Top/>
      <Bottom/>
    </main>
    <Foooter/>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'

import Header from './components/Header.vue'
import Top from './components/Top.vue'
import Bottom from './components/Bottom.vue'
import Foooter from './components/Foooter.vue'

export default {
  name: 'App',
  components: {
    Header,
    Top,
    Bottom,
    Foooter
  }
}
</script>

<style lang="scss">
  @import "@/assets/style/common";
</style>
