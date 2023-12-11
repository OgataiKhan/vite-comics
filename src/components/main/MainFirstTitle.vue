<script>


export default {
  name: 'FirstTitle',

};

</script>

<template>
  <h2>Current Series</h2>
</template>

<style lang="scss" scoped>
@use '../../styles/partials/variables.scss' as *;

h2 {
  text-transform: uppercase;
  padding: 10px 30px;
  background-color: $secondary-color;
  display: inline-block;
  transform: translateY(-30px);
  font-size: 1.7rem;
}
</style>