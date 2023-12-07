<script>


export default {
  name: 'FooterBottom',
  data() {
    return {
      socials: [
        {
          socialName: 'Facebook',
          iconPath: '../../../src/assets/footer-facebook.png',
        },
        {
          socialName: 'Twitter',
          iconPath: '../../../src/assets/footer-twitter.png',
        },
        {
          socialName: 'Youtube',
          iconPath: '../../../src/assets/footer-youtube.png',
        },
        {
          socialName: 'Pinterest',
          iconPath: '../../../src/assets/footer-pinterest.png',
        },
        {
          socialName: 'Periscope',
          iconPath: '../../../src/assets/footer-periscope.png',
        },
      ],
    };
  },
};

</script>

<template>
  <div class="footer-bottom">
    <div class="container">
      <p class="footer-bottom-left">Sign-up now!</p>
      <div class="footer-bottom-right">
        <p>Follow us</p>
        <ul class="social-list">
          <li v-for="social in socials">
            <a href="#">
              <img :src="social.iconPath" :alt="social.socialName">
            </a>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use '../../styles/partials/variables.scss' as *;
@use '../../styles/general.scss' as *;

.footer-bottom {
  background-color: #303030;
  text-transform: uppercase;
  font-weight: 500;
}

.container {
  @include container;
  display: flex;
  justify-content: space-between;

  .footer-bottom-left {
    display: flex;
    align-items: center;
    border: 2px solid $secondary-color;
    padding: 14px;
    margin: 30px 0;
    cursor: pointer;
  }
  .footer-bottom-right {
    display: flex;
    align-items: center;
    p {
      color: $secondary-color;
      padding-right: 30px;
    }
    .social-list {
      display: flex;
      gap: 19px;
      li {
        width: 35px;
      }
    }
  }
}
</style>