<template>
  <div>
    <div id="nav">
      <ul>
        <li><router-link to="/">Home</router-link></li>
        <li><router-link to="/about">About</router-link></li>
        <li><router-link to="/skills">skills</router-link></li>
        <li><router-link to="/portofllo">portofllo</router-link></li>
      </ul>

      <div class="info">
        <div class="content">
          <div class="imgBx">
            <img alt="Vue logo" :src="require('@/imags/bg.jpg')" />
          </div>
          <div class="textBx">
            <h2>Omar Mohamed <span>Thomas</span></h2>
            <p>Fullstack Web Developer.</p>
            <a href="#">Downlode CV</a>
          </div>
          <div class="sci">
            <ul>
              <li>
                <a href="https://www.facebook.com/profile.php?id=100011178858933"><img :src="require('@/imags/facebook.png')"/></a>
              </li>
              <li>
                <a href="https://www.instagram.com/thomasmahamed/" class="mr"><img :src="require('@/imags/instagram.png')"/></a>
              </li>
              <li>
                <a href="https://twitter.com/Thomas62004808"><img :src="require('@/imags/twitter.png')"/></a>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Nav",
  data() {
    return {
      imgPath: require("@/imags/bg.jpg"),
      faceboox: require("@/imags/facebook.png"),
      instagram: require("@/imags/instagram.png"),
      twitter: require("@/imags/twitter.png"),
    };
  },
};
</script>

<style lang="scss">
#nav {
  padding: 30px;
  position: absolute;
  top: 0;
  left: 0;
  width: 25%;
  height: 100vh;
  background: #2c3e50;
  z-index: 10;
  ul {
    width: 90%;
    display: flex;
  }

  a {
    font-weight: 500;
    color: #fff;
    margin-right: 30px;
    font-size: 20px;
    &.router-link-exact-active {
      color: #42b983;
    }
  }
}

.info {
  position: relative;
  margin-top: 50px;
  .content {
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    .imgBx {
      position: relative;
      width: 300px;
      height: 300px;
      padding-bottom: 20px;
      border-radius: 50%;
      overflow: hidden;
      box-shadow: Rgb(100 100 111 / 20%) 7px -7px 14px 8px;
      margin-bottom: 20px;
      img {
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        object-fit: cover;
      }
    }
    .textBx {
      position: relative;
      max-width: 500px;
      text-align: center;
      h2 {
        color: #fff;
        font-weight: 700;
        span {
          color: #42b983;
        }
      }
      p {
        color: #ccc;
        font-size: 20px;
        margin: 20px 0 30px;
      }
      a {
        color: #fff;
        background: #42b983;
        text-decoration: none;
        border-radius: 50px;
        padding: 10px 20px;
        margin: 0 !important;
      }
    }
    .sci {
      position: relative;
      margin-top: 70px;
      li {
        list-style: none;
        .mr{margin: 0 30px !important;}
        a {
          text-decoration: none;
          filter: invert(1);
          margin: 0 !important;
          img {
            max-width: 100px;
            transform: scale(0.8);
            opacity: 0.7;
            transition: all 0.3s ease-in-out;
            &:hover {
              opacity: 1;
              transform: scale(1.2);
            }
          }
        }
      }
    }
  }
}
</style>
