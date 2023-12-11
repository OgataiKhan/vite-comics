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
      <Section1 />
    </div>
  </main>
</template>

<style lang="scss" scoped>
@use '../styles/partials/mixins.scss' as *;

main {
  font-size: 1.5rem;
}

.container {
  @include container;
}

.jumbo {
  aspect-ratio: 5;
  overflow: hidden;
}
</style>