<template>
  <section class="section">
    <div class="columns" style="flex-wrap: wrap">
      <RestaurantCard />
    </div>
    <div class="columns">
      <div class="column">
        <nuxt-link to="/admin" class="button is-info">
          Admin
        </nuxt-link>
      </div>
    </div>
  </section>
</template>

<script>
import RestaurantCard from '~/components/RestaurantCard'
export default {
  components: {
    RestaurantCard
  },
  data() {
    return {}
  }
}
</script>

<style></style>
