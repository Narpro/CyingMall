<template>
  <div id="app">
    <router-view/>
    <TabBar></TabBar>
  </div>
</template>

<script>
import TabBar from './components/content/MainBar'
export default {
  name: 'app',
  components: {
    TabBar
  }
}
</script>

<style>
@import "assets/css/base.css"
</style>
