<template>
  <div id="home">
    <div class="header">
      <div class="vertical_line"></div>

      <div class="user_info">
        <img class="user_photo" src="https://avatars.githubusercontent.com/u/23065460?v=4" alt="user photo">
        <h2>Jemima Luz</h2>
        <div class="horizontal_line"></div>

        <nav class="links">
          <a href="">
            <GitIcon/>
          </a>
          <a href="">
            <LinkedinIcon/>

          </a>
          <a href="">
            <WebIcon/>

          </a>
        </nav>
      </div>
    </div>

    <div class="footer">
      <p>quer saber mais? vem!</p>
      <div></div>
      <nav>
        <a href="">Git</a>
        <a href="">Lnkd</a>
        <a href="">Web</a>
      </nav>
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
import GitIcon from './components/GitHubIcon.vue'
import WebIcon from './components/WebIcon.vue'
import LinkedinIcon from './components/LinkedinIcon.vue'

@Component({
  components: {
    GitIcon,
    WebIcon,
    LinkedinIcon
  },
})
export default class Home extends Vue {}
</script>

<style lang="scss">
  @import "../styles/styles.scss";

  #home {
    .header {
      .user_info {
        .user_photo { @include userPhoto; }
        h2 { @include userNameFont; }
        .horizontal_line { @include horizontalLineShape; }

        .links {
          display: flex;
          flex-direction: row;

          a {
            padding: 8px;
            background-color: $almostWhite;

            display: flex;
            align-items: center;
          }
        }
      }
    }

    .footer {

    }
  }
</style>
