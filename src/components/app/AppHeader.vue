<template>
  <div>
    <div class="header">
      <h1 class=" wow animate__fadeInLeft" data-wow-duration="1" data-wow-delay="0.001s">{{ name }}</h1>
    </div>
  </div>
</template>

<script>
import { WOW } from "wowjs";

export default {
  name: "AppHeader",
	props: {
		name: String,
	},
  mounted() {
    var wow = new WOW({
      boxClass: "wow",
      animateClass: "animated",
      offset: 0,
      mobile: true,
    });
    wow.init();
  }
}
</script>

<style lang="scss">
.header {
  position: absolute;
  top: 0;
  left: 25%;
  background: #42b983;
  width: 75%;
  z-index: 9;
  h1 {
    margin: 0 20px;
    color: #fff;
    padding: 20px 10px;
  }
}
</style>
