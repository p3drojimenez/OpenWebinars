<template>
  <section class="section">
    <div class="container">
      <div class="column">
        <RestaurantCard />
        {{ message }}
      </div>
      <div class="column">
        <nuxt-link to="/admin" class="button is-info">
          Admin
        </nuxt-link>
      </div>
    </div>
  </section>
</template>

<script>
import RestaurantCard from "~/components/RestaurantCard.vue"

export default {
  components: {
    RestaurantCard
  },
  data() {
    return {
      message: "hola mundo!"
    }
  }
}
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
