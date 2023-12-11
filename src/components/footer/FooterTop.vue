<script>


export default {
  name: 'FooterTop',
  data() {
    return {
      links: [
        {
          icon: 'Digital Comics',
          iconPath: '../../../src/assets/buy-comics-digital-comics.png',
        },
        {
          icon: 'DC Merchandise',
          iconPath: '../../../src/assets/buy-comics-merchandise.png',
        },
        {
          icon: 'Subscription',
          iconPath: '../../../src/assets/buy-comics-subscriptions.png',
        },
        {
          icon: 'Comic Shop Locator',
          iconPath: '../../../src/assets/buy-comics-shop-locator.png',
        },
        {
          icon: 'DC Power Visa',
          iconPath: '../../../src/assets/buy-dc-power-visa.svg',
        },
      ],
    };
  },
};

</script>

<template>
  <div class="footer-top">
    <div class="container">
      <ul class="banner-link-list">
        <li v-for="link in links">
          <a href="#">
            <div class="banner-icon">
              <img :src="link.iconPath" :alt="link.icon">
            </div>
            <p>
              {{ link.icon }}
            </p>
          </a>
        </li>
      </ul>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use '../../styles/partials/variables.scss' as *;
@use '../../styles/partials/mixins.scss' as *;

.footer-top {
  background-color: $secondary-color;
  font-family: 'Asap', sans-serif;
}

.container {
  @include container;

  .banner-link-list {
    display: flex;
    justify-content: space-around;
    padding: 50px 0;

    li {
      display: flex;
      align-items: center;

      a {
        display: flex;
        align-items: center;
        gap: 17px;
        text-decoration: none;
        color: $base-font;
        text-transform: uppercase;
        vertical-align: middle;

        .banner-icon {
          width: 50px;
          height: 50px;
          img {
            height: 100%;
            object-fit: contain;
          }
        }
      }
    }


  }
}</style>