<script>


export default {
  name: 'FooterMid',
};

</script>

<template>
  <div class="footer-mid">
    <div class="container">
      <div>
        <h4>DC comics</h4>
        <ul>
          <li>Placeholder</li>
          <li>Placeholder</li>
          <li>Placeholder</li>
          <li>Placeholder</li>
        </ul>
        <h4 class="footerlisttitle-shop">Shop</h4>
        <ul>
          <li>Placeholder</li>
          <li>Placeholder</li>
          <li>Placeholder</li>
          <li>Placeholder</li>
        </ul>
      </div>
      <div>
        <h4>DC</h4>
        <ul>
          <li>Placeholder</li>
          <li>Placeholder</li>
          <li>Placeholder</li>
          <li>Placeholder</li>
        </ul>
      </div>
      <div>
        <h4>Sites</h4>
        <ul>
          <li>Placeholder</li>
          <li>Placeholder</li>
          <li>Placeholder</li>
          <li>Placeholder</li>
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
  list-style: none;
  padding-right: 30px;
  li {
    line-height: 1.5;
    font-weight: 400;
    font-size: 0.9rem;
    color: #959595;
  }
}

.footerlisttitle-shop {
    padding-top: 20px;
  }

</style>