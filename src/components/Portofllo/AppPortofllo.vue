<template>
  <div class="appPortofllo">
    <div class="content">
      <div
        class="bar wow animate__fadeInDown"
        data-wow-duration="1"
        data-wow-delay="0.3s"
      >
        <ul>
          <li>All</li>
          <li>Personal pages</li>
          <li>Product Pages</li>
          <li>js Projects</li>
          <li>
            Restaurants pages
          </li>
        </ul>
      </div>
      <div
        class="imgBx d-flex flex-wrap wow animate__fadeInUp"
        data-wow-duration="1"
        data-wow-delay="0.3s"
      >
        <div class="image all">
          <img :src="require('@/imags/bg1.jpg')" class="" />
          <div class="textBx">
            <h3>Project 01</h3>
          </div>
        </div>
        <div class="image all">
          <img :src="require('@/imags/bg2.jpg')" class="" />
          <div class="textBx">
            <h3>Project 02</h3>
          </div>
        </div>
        <div class="image all">
          <img :src="require('@/imags/bg3.jpg')" class="" />
          <div class="textBx">
            <h3>Project 03</h3>
          </div>
        </div>
        <div class="image all">
          <img :src="require('@/imags/bg1.jpg')" class="" />
          <div class="textBx">
            <h3>Project 04</h3>
          </div>
        </div>
        <div class="image all">
          <img :src="require('@/imags/bg2.jpg')" class="" />
          <div class="textBx">
            <h3>Project 05</h3>
          </div>
        </div>
        <div class="image all">
          <img :src="require('@/imags/bg3.jpg')" class="" />
          <div class="textBx">
            <h3>Project 06</h3>
          </div>
        </div>
        <div class="image all">
          <img :src="require('@/imags/bg1.jpg')" class="" />
          <div class="textBx">
            <h3>Project 07</h3>
          </div>
        </div>
        <div class="image all">
          <img :src="require('@/imags/bg2.jpg')" class="" />
          <div class="textBx">
            <h3>Project 08</h3>
          </div>
        </div>
        <div class="image all">
          <img :src="require('@/imags/bg3.jpg')" class="" />
          <div class="textBx">
            <h3>Project 09</h3>
          </div>
        </div>
        <div class="image all">
          <img :src="require('@/imags/bg1.jpg')" class="" />
          <div class="textBx">
            <h3>Project 10</h3>
          </div>
        </div>
        <div class="image all">
          <img :src="require('@/imags/bg2.jpg')" class="" />
          <div class="textBx">
            <h3>Project 11</h3>
          </div>
        </div>
        <div class="image all">
          <img :src="require('@/imags/bg3.jpg')" class="" />
          <div class="textBx">
            <h3>Project 12</h3>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import { WOW } from "wowjs";

export default {
  name: "appPortofllo",
  data() {
    return {
      imgPath: require("@/imags/bg1.jpg"),
      imgPath2: require("@/imags/bg2.jpg"),
      imgPath3: require("@/imags/bg3.jpg"),
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
.appPortofllo {
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
  }
  .bar {
    width: 100%;
    text-align: center;
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 30px;
    ul {
      display: flex;
      justify-content: center;
      align-items: center;
      .active {
        color: #42b983;
      }
      li {
        list-style: none;
        color: #fff;
        margin-right: 30px;
        font-size: 18px;
        transition: 0.5s;
        cursor: pointer;
        &:hover {
          color: #42b983;
        }
      }
    }
  }
  .imgBx {
    width: 100%;
    padding: 10px 30px;
    .image {
      margin: 20px 0 0 20px;
      img {
        width: 300px;
        opacity: 0.7;
        transition: 0.5s;
        &:hover {
          opacity: 1;
        }
      }
    }
    .textBx {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      display: flex;
      justify-content: center;
      align-items: center;
      background-color: Rgb(0 0 0 / 80%);
      opacity: 0;
      transition: all 0.7s ease-in-out;
      h3 {
        color: #fff;
        text-transform: uppercase;
        letter-spacing: 1px;
        font-size: 1em;
      }
      &:hover {
        opacity: 1;
      }
    }
  }
}
</style>
