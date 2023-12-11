<script>


export default {
  name: 'MainComponent',
};

</script>

<template>
  <main>
    <div class="container">
    --&gt; Content goes here &lt;--
    </div>
  </main>
</template>

<style lang="scss" scoped>
@use '../styles/partials/mixins.scss' as *;

main {
  height: 200px;
  font-size: 1.5rem;
}

.container {
  @include container;
}
</style>