<script>
import HeaderComponent from './components/Header.vue';
import MainComponent from './components/Main.vue';
import FooterComponent from './components/Footer.vue';

export default {
  name: 'AppComponent',
  components: {
    HeaderComponent,
    MainComponent,
    FooterComponent,
  },
};
</script>

<template>
  <HeaderComponent />
  <MainComponent />
  <FooterComponent />
</template>

<style lang="scss">
@use './styles/partials/variables.scss' as *;
@use './styles/general.scss' as *;

</style>
