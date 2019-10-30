<template>
  <section class="section">
    <div class="columns" style="flex-wrap: wrap">
      <div
        class="column"
        style="margin: 20"
        v-for="(restaurant, index) in restaurants"
        :key="index"
      >
        <RestaurantCard />
      </div>
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
    return {
      restaurants: [
        {
          name: 'Manairo',
          slug: 'manairo'
        },
        {
          name: 'Gorría Restaurant',
          slug: 'gorria-restaurant'
        },
        {
          name: 'Dans le Noir?',
          slug: 'dans-noir'
        }
      ]
    }
  }
}
</script>

<style></style>
