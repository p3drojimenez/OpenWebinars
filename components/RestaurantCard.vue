<template>
  <div class="card" style="width:400px;">
    <div class="card-image">
      <figure class="image">
        <img src="~/assets/images/pizza.jpg" alt="Pizza Restaurant" />
      </figure>
    </div>
    <div class="card-content">
      <div class="media">
        <div class="media-content">
          <p class="title is-4 restaurant-name">
            {{ name }}
          </p>
          <p class="subtitle is-6">
            <span class="is-category tag">{{ category }}</span>
            <span class="tag is-info" v-if="likes != 0">{{ likes }}</span>
            <span class="tag is-warning" v-else>NO TIENE LIKES</span>
          </p>
        </div>
      </div>
      <div class="content">
        {{ description }}
      </div>
      <div>
        <!-- <ul>
          <li v-for="(item, index) in items" :key="index"> {{ item }}</li>
        </ul> -->
        <ul>
          <li v-for="(restaurant, index) in restaurants" :key="index">
            <button @click="goToRestaurant(restaurant.slug)">
              {{ restaurant.name }}
            </button>
          </li>
        </ul>
        <button class="button" @click="sumLikes">sumar like</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      name: 'Restaurante Italiano',
      category: "Italian",
      description: "the best italian restaurant in Barcelona.",
      likes: 0,
      items: ['Peras', 'Manzanas', 'Platanos'],
      restaurants: [
        {
          name: "Manairo",
          slug: "manairo"
        },
        {
          name: "Gorría Restaurant",
          slug: "gorria-restaurant"
        },
        {
          name: "Dans le Noir?",
          slug: "dans-noir"
        }
      ]
    }
  },
  methods: {
    sumLikes() {
      this.likes = this.likes + 1
    },
    goToRestaurant(slug) {
      this.$router.push(slug)
    }
  }
}
</script>

<style>
.restaurant-name {
  font-family: 'Pacifico';
  font-size: 30px;
  color: #8ae6ff;
}
</style>