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
            La real Burger
          </p>
          <p class="subtitle is-6">
            <span class="is-category tag">
              Burgers
            </span>
          </p>
        </div>
      </div>
      <div class="content">
        <p>
          The best italian restaurant in Barcelona
        </p>
      </div>
      <div class="columns">
        <div class="column">
          <button class="button" @click="onLikeButton">
            <span class="icon is-small">
              <font-awesome-icon :icon="['fa', 'heart']" style="color: #red;" />
            </span>
          </button>
        </div>
        <div class="column">
          <button class="button is-info" v-on:click="onDetailBoton">
            More Info
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
<<<<<<< HEAD
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
=======
}
</script>

<style lang="scss" scoped>
>>>>>>> restaurantcomponent
.restaurant-name {
  font-family: 'Pacifico';
  font-size: 30px;
  color: #8ae6ff;
}
<<<<<<< HEAD
</style>
=======
</style>
>>>>>>> restaurantcomponent
