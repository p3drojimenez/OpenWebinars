<template>
  <section class="section">
<<<<<<< HEAD
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
=======
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
>>>>>>> restaurantcomponent
  </section>
</template>

<script>
<<<<<<< HEAD
import RestaurantCard from "~/components/RestaurantCard.vue"

=======
import RestaurantCard from '~/components/RestaurantCard'
>>>>>>> restaurantcomponent
export default {
  components: {
    RestaurantCard
  },
  data() {
    return {
<<<<<<< HEAD
      message: "hola mundo!"
=======
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
>>>>>>> restaurantcomponent
    }
  }
}
</script>

<style></style>
