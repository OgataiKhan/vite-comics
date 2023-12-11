<script>


export default {
  name: 'Product',
  props: ['thumb', 'series'],
};

</script>

<template>
  <li class="product-card">
    <div class="product">
      <div class="product-img">
        <img :src="thumb" :alt="series">
      </div>
      <p>{{ series }}</p>
    </div>
  </li>
</template>

<style lang="scss" scoped>

</style>