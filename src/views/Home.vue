<template>
  <div class="home">
    <AppHeader name="Home"/>
    <AppHome />
  </div>
</template>

<script>
// @ is an alias to /src
import AppHeader from '@/components/app/AppHeader.vue'
import AppHome from '@/components/Home/AppHome.vue'

export default {
  name: "Home",
  components: {
    AppHeader,
    AppHome
  }
};
</script>

<style lang="scss">

</style>
