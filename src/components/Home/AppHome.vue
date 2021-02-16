<template>
  <div class="appHome">
    <div class="content">
      <div
        class="textBx wow slideInRight"
        data-wow-duration="1"
        data-wow-delay="0.3s"
      >
        <h2>Welcome</h2>
        <p>
          My name is Omar Mohamed <br />
          <span>I'm a fullstack web developer and freelancer, this is my page to
          introduction me.</span>
        </p>
      </div>
    </div>
  </div>
</template>

<script>
import { WOW } from "wowjs";

export default {
  name: "AppHome",
  data() {
    return {
      imgPath: require("@/imags/bg3.jpg"),
    };
  },
  mounted() {
    var wow = new WOW({
      boxClass: "wow",
      animateClass: "animated",
      offset: 0,
      mobile: true,
    });
    wow.init();
  },
};
</script>

<style lang="scss">
.appHome {
  position: absolute;
  top: 0;
  left: 25%;
  width: 75%;
  height: 100vh;
  .content {
    max-width: 100%;
    height: calc(90vh - 5px);
    margin-top: 88px;
    background-color: #2c3e5069;
    .textBx {
      z-index: 11;
      padding: 30px;
      display: flex;
      justify-content: center;
      align-items: center;
      flex-direction: column;
      text-align: center;
      height: 100%;
      h2 {
        color: #42b983;
        font-weight: 700;
        letter-spacing: 2px;
        font-size: 6rem;
      }
      p {
        color: #ffffffc2;
        font-size: 25px;
        // span{
        //   color: #42b983;
        // }
      }
    }
  }
}
</style>
