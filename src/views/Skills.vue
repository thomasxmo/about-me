<template>
  <div class="skills">
    <AppHeader name="Skills"/>
    <AppSkills />
  </div>
</template>

<script>
// @ is an alias to /src
import AppHeader from '@/components/app/AppHeader.vue'
import AppSkills from '@/components/Skills/AppSkills.vue'

export default {
  name: "skills",
  components: {
    AppHeader,
    AppSkills
  }
};
</script>