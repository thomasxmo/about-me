<template>
  <div class="about">
    <AppHeader name="About"/>
    <AppAbout />
  </div>
</template>

<script>
// @ is an alias to /src
import AppHeader from '@/components/app/AppHeader.vue'
import AppAbout from '@/components/about/AppAbout.vue'

export default {
  name: "about",
  components: {
    AppHeader,
    AppAbout
  }
};
</script>