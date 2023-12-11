<script>
import Jumbotron from './main/MainJumbo.vue';
import Section1 from './main/MainSection1.vue';

export default {
  name: 'MainComponent',
  components: {
    Jumbotron,
    Section1,
  }
};

</script>

<template>
  <main>
    <Jumbotron />
    <div class="container">
      <h2>Current Series</h2>
    --&gt; Content goes here &lt;--
    </div>
  </main>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables.scss' as *;
@use '../styles/partials/mixins.scss' as *;

main {
  font-size: 1.5rem;
}

.container {
  @include container;
  h2 {
    text-transform: uppercase;
    padding: 10px 30px;
    color: $base-font;
    background-color: $secondary-color;
    display: inline-block;
    transform: translateY(-30px);
  }
}

.jumbo {
  aspect-ratio: 5;
  overflow: hidden;
}
</style>