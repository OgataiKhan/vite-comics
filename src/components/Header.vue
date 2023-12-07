<script>


export default {
  name: 'HeaderComponent',
};

</script>

<template>
  <header>
    <div class="container">
      <div class="logo">
        <img src="../assets/dc-logo.png" alt="DC Logo">
      </div>
      <nav class="navbar">
        <ul class="header-menu">
          <li>
            <a href="#">Placeholder</a>
          </li>
          <li>
            <a href="#">Placeholder</a>
          </li>
          <li>
            <a href="#">Placeholder</a>
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables.scss' as *;
@use '../styles/general.scss' as *;

header {
  background-color: #FFFFFF;
}

.container {
  @include container;
  @include flex-justify-center;
  align-items: stretch;
}

.logo {
  width: 80px;
  padding: 19px 0;
}

.header-menu {
  display: flex;
  height: 100%;
  align-items: center;
  gap: 33px;
  text-transform: uppercase;
  font-weight: 500;

  li {
    height: 100%;
    display: flex;
    align-items: center;
    border-top: 5px solid transparent;
    border-bottom: 5px solid transparent;

    &:hover {
      border-bottom: 5px solid $secondary-color;
      cursor: pointer;
      a {
        color: $secondary-color;
      }
    }

    a {
      color: #464646;
      text-decoration: none;
    }
  }
}
</style>