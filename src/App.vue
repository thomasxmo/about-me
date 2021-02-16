<template>
  <div id="app">
    <AppNav />
    <router-view />
  </div>
</template>

<script>
// @ is an alias to /src
import AppNav from './components/app/AppNav.vue'

export default {
  name: 'app',
   components: {
    AppNav
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
</style>
