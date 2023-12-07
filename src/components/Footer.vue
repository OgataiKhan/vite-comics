<script>
import FooterTop from './footer/FooterTop.vue';
import FooterMid from './footer/FooterMid.vue';
import FooterBottom from './footer/FooterBottom.vue';

export default {
  name: 'FooterComponent',
  components: {
    FooterTop,
    FooterMid,
    FooterBottom,
  }
};

</script>

<template>
  <footer>
    <FooterTop />
    <FooterMid />
    <FooterBottom />
  </footer>
</template>

<style scoped></style>