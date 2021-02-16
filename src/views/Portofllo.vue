<template>
  <div class="portofllo">
    <AppHeader name="Portofllo" />
    <AppPortofllo />
  </div>
</template>

<script>
// @ is an alias to /src
import AppHeader from "@/components/app/AppHeader.vue";
import AppPortofllo from "@/components/Portofllo/AppPortofllo.vue";

export default {
  name: "portofllo",
  components: {
    AppHeader,
    AppPortofllo,
  },
};
</script>
