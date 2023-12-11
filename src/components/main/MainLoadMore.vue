<script>


export default {
  name: 'LoadMore',

};

</script>

<template>
  <div class="btn-subsection">
    <button>Load more</button>
  </div>
</template>

<style lang="scss" scoped>
@use '../../styles/partials/variables.scss' as *;

.btn-subsection {
  text-align: center;
  padding-bottom: 20px;

  button {
    text-transform: uppercase;
    padding: 10px 60px;
    background-color: $secondary-color;
    display: inline-block;
    font-size: 1rem;
    color: $base-font;
    border: none;
    cursor: pointer;
  }
}
</style>