<script>


export default {
  name: 'FooterMid',
  data() {
    return {
      listDccomics: ['Characters', 'Comics', 'Movies', 'TV', 'Games', 'Videos', 'News'],
      listShop: ['Shop DC', 'Shop DC Collectibles'],
      listDc: ['Terms Of Use', 'Privacy Policy (New)', 'Ad Choices', 'Advertising', 'Jobs', 'Subscriptions', 'Talent Workshops', 'CPSC Certificates', 'Ratings', 'Shop Help', 'Contact Us'],
      listSites: ['DC', 'MAD Magazine', 'DC Kids', 'DC Universe', 'DC Power Visa'],
    };
  },
};

</script>

<template>
  <div class="footer-mid">
    <div class="container">
      <div>
        <h4>DC comics</h4>
        <ul>
          <li v-for="item in listDccomics">
            <a href="#">{{ item }}</a>
          </li>
        </ul>
        <h4 class="footerlisttitle-shop">Shop</h4>
        <ul>
          <li v-for="item in listShop">
            <a href="#">{{ item }}</a>
          </li>
        </ul>
      </div>
      <div>
        <h4>DC</h4>
        <ul>
          <li v-for="item in listDc">
            <a href="#">{{ item }}</a>
          </li>
        </ul>
      </div>
      <div>
        <h4>Sites</h4>
        <ul>
          <li v-for="item in listSites">
            <a href="#">{{ item }}</a>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
// @use '../../styles/partials/variables.scss' as *;
@use '../../styles/general.scss' as *;

.container {
  @include container;
  display: flex;
  padding: 45px 0;
}

h4 {
  text-transform: uppercase;
  padding-bottom: 15px;
  font-size: 1.3rem;
}

ul {
  padding-right: 30px;
  li a {
    line-height: 1.5;
    font-weight: 400;
    font-size: 0.9rem;
    color: #959595;
    text-decoration: none;
  }
}

.footerlisttitle-shop {
    padding-top: 20px;
  }

</style>