<script>


export default {
  name: 'FooterTop',
};

</script>

<template>
  <div class="footer-top">
    <div class="container">
      Footer Top
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use '../../styles/partials/variables.scss' as *;
@use '../../styles/general.scss' as *;

.footer-top {
  height: 100px;
  background-color: $secondary-color;
  font-family: 'Asap', sans-serif;
}

.container {
  @include container;
}

</style>