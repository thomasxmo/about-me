<template>
  <div class="appabout">
    <div class="content">
      <div class="row">
        <div class="col-md-12 Desigen">
          <h2>Desigen Skills</h2>
          <div class="row">
            <div
              class="skillBx col-md-6 wow animate__fadeInLeft"
              data-wow-duration="1"
              data-wow-delay="0.3s"
            >
              <h3>HTML</h3>
              <div>
                <span style="width: 90%;">90% &nbsp;</span>
              </div>
              <h3>CSS</h3>
              <div>
                <span style="width: 90%;">90% &nbsp;</span>
              </div>
              <h3>Javascript</h3>
              <div>
                <span style="width: 70%;"> 70% &nbsp;</span>
              </div>
              <h3>VUE</h3>
              <div>
                <span style="width: 60%;"> 60% &nbsp;</span>
              </div>
            </div>
            <div
              class="skillBx col-md-6 wow animate__fadeInRight"
              data-wow-duration="1"
              data-wow-delay="0.3s"
            >
              <h3>Jqury</h3>
              <div>
                <span style="width: 40%;"> 40% &nbsp;</span>
              </div>
              <h3>SASS</h3>
              <div>
                <span style="width: 85%;"> 85% &nbsp;</span>
              </div>
              <h3>Bootstrip</h3>
              <div>
                <span style="width: 90%;"> 90% &nbsp;</span>
              </div>
              <h3>Gulpjs</h3>
              <div>
                <span style="width: 60%;"> 60% &nbsp;</span>
              </div>
            </div>
          </div>
        </div>
        <div class="col-md-12 development">
          <h2>development Skills</h2>
          <div
            class="skillBx wow animate__fadeInBottomLeft"
            data-wow-duration="1"
            data-wow-delay="0.3s"
          >
            <div class="row">
              <div class="col-md-6 ">
                <h3>Python</h3>
                <div class="md">
                  <span style="width: 70%;"> 70% &nbsp;</span>
                </div>
              </div>

              <div class="col-md-6">
                <h3>SQL</h3>
                <div class="md">
                  <span style="width: 85%;"> 85% &nbsp;</span>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import { WOW } from "wowjs";

export default {
  name: "appabout",
  data() {
    return {
      imgPath: require("@/imags/bg3.jpg"),
      number: null,
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
.appabout {
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
    padding: 10px 30px;
  }
  .Desigen {
    padding: 30px;
    margin-bottom: 5px;
    h2 {
      color: #42b983;
      margin-bottom: 20px;
    }
    .skillBx {
      width: 100%;
      h3 {
        color: #fff;
      }
      span {
        display: block;
        margin-bottom: 20px;
        color: #fff;
        background: #42b983;
        text-align: right;
        border-radius: 1px;
        padding: 3px 7px;
      }
      div {
        background-color: #2c3e507d;
      }
    }
  }
  .development {
    padding: 30px;
    margin-bottom: 5px;
    h2 {
      color: #42b983;
      margin-bottom: 20px;
    }
    .skillBx {
      width: 100%;
      h3 {
        color: #fff;
      }
      span {
        display: block;
        margin-bottom: 20px;
        color: #fff;
        background: #42b983;
        text-align: right;
        border-radius: 1px;
        padding: 3px 7px;
      }
      .md {
        background-color: #2c3e507d;
      }
    }
  }
}
</style>
