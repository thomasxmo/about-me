<template>
  <div class="appabout">
    <div class="content">
      <div class="row">
        <div
          class="info col-md-6 wow animate__fadeInLeft"
          data-wow-duration="1"
          data-wow-delay="0.3s"
        >
          <h2>Informations about me</h2>
          <table class="rwd-table">
            <tr>
              <th>question</th>
              <th>answer</th>
            </tr>
            <tr>
              <td data-th="Movie Title">Name</td>
              <td data-th="Genre">omar mohamed</td>
            </tr>
            <tr>
              <td data-th="Movie Title">Niakname</td>
              <td data-th="Genre">"thomas"</td>
            </tr>
            <tr>
              <td data-th="Movie Title">Adg</td>
              <td data-th="Genre">16</td>
            </tr>
            <tr>
              <td data-th="Movie Title">country</td>
              <td data-th="Genre">Egypt</td>
            </tr>
            <tr>
              <td data-th="Movie Title">Work</td>
              <td data-th="Genre">freelancer</td>
            </tr>
            <tr>
              <td data-th="Movie Title">Degree</td>
              <td data-th="Genre">Certificate of Secondary Education</td>
            </tr>
            <tr>
              <td data-th="Movie Title">specialty</td>
              <td data-th="Genre">Web page programmer</td>
            </tr>
          </table>
        </div>
        <div
          class="info col-md-6 wow animate__fadeInRight"
          data-wow-duration="1"
          data-wow-delay="0.3s"
        >
          <h2>Other things</h2>
          <table class="rwd-table">
            <tr>
              <th>favorite</th>
              <th>thing</th>
            </tr>
            <tr>
              <td data-th="Movie Title">Movie</td>
              <td data-th="Genre">The Shawshank Redemption (1994)</td>
            </tr>
            <tr>
              <td data-th="Movie Title">songe</td>
              <td data-th="Genre">Fly me to the moon</td>
            </tr>
            <tr>
              <td data-th="Movie Title">anime</td>
              <td data-th="Genre">HxH, Attack on Titan, naruto and one pice</td>
            </tr>
            <tr>
              <td data-th="Movie Title">TV series</td>
              <td data-th="Genre">Friends (1994)</td>
            </tr>
            <tr>
              <td data-th="Movie Title">country</td>
              <td data-th="Genre">Japan</td>
            </tr>
            <tr>
              <td data-th="Movie Title">Singer</td>
              <td data-th="Genre">Frank Sinatra</td>
            </tr>
            <tr>
              <td data-th="Movie Title">actor</td>
              <td data-th="Genre">Leonardo DiCaprio</td>
            </tr>
          </table>
        </div>
        <div
          class="col-md-12 contact wow animate__fadeInBottomLeft"
          data-wow-duration="1"
          data-wow-delay="0.3s"
        >
          <ul>
            <li>Email : <span>omarx2005@gmail.com</span></li>
            <li>Phone : <span>+201017061753</span></li>
            <li>
              GitHub :
              <span><a href="https://github.com/thomasxmo">thomasxmo</a></span>
            </li>
          </ul>
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
    .info {
      padding: 0px 30px;
      h2 {
        color: #fff;
        margin-bottom: 20px;
      }
      .rwd-table {
        background: #34495e33;
        color: #fff;
        border-radius: 0.4em;
        overflow: hidden;
        width: 100%;
        box-shadow: Rgb(0 0 0 / 10%) 14px 12px 9px;
        tr {
          border-color: lighten(#34495e, 10%);
        }
        th,
        td {
          margin: 0.5em 1em;
          padding: 1em !important;
        }
        th,
        td:before {
          color: #42b983;
        }
      }
    }
    .contact {
      max-width: 95%;
      box-shadow: Rgb(0 0 0 / 10%) 14px 12px 9px;
      background: #34495e33;
      color: #fff;
      border-radius: 0.4em;
      overflow: hidden;
      margin: 30px auto 0;
      padding: 30px;
      ul {
        display: flex;
        justify-content: space-between;
        align-items: center;
        li {
          list-style: none;
          font-size: 18px;
          span {
            color: #42b983;
            a {
              text-decoration: none;
              color: #42b983;
            }
          }
        }
      }
    }
  }
}
</style>
