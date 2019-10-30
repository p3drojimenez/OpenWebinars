<template>
  <nav class="navbar" role="navigation" aria-label="main navigation">
    <div class="navbar-brand logo">
      <img src="~/assets/images/logo.png" alt="FoodAdvisor logo" />
    </div>
    <div class="navbar-end">
      <div class="navbar-item">
        <nuxt-link to="login" class="button custom-button">
          Login
        </nuxt-link>
      </div>
    </div>
  </nav>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
@import '~/assets/css/variables.scss';
.logo {
  width: 100px;
  margin: 0 20px;
}
.navbar {
  border-bottom: 2px solid $secondary;
}
.custom-button {
  color: white;
  background-color: $primary;
  &:hover {
    background-color: darken($primary, 20);
  }
}
</style>
