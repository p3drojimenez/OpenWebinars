<template>
  <div class="box column is-4 is-offset-4 box-login">
    <div class="columns">
      <div class="column has-text-centered">
        <h2 class="title is-2">Order Food</h2>
      </div>
    </div>
    <div class="columns">
      <div class="column has-text-left">
        <label>Name</label>
        <input class="input" type="text" placeholder="name" />
      </div>
    </div>
    <div class="columns box" style="margin: 10px">
      <div class="column">
        <div class="columns">
          <div class="column has-text-centered">
            <p>
              <strong>Pizza Napilitana</strong>
            </p>
          </div>
        </div>
        <div class="columns">
          <div class="column">
            <img src="~/assets/images/pizza_napolitana.jpg" class="img-pizza" />
          </div>
          <div class="column">
            <ul>
              <li>Albahaca fresca</li>
              <li>Tomates</li>
              <li>mozzarella</li>
              <li>Aceite de oliva virgen extra</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
    <div class="columns">
      <div class="column has-text-left">
        <div class="field">
          <label class="label">Units</label>
          <div class="control">
            <input
              class="input"
              type="text"
              v-model="units"
              placeholder="units"
            />
          </div>
        </div>
      </div>
      <div class="column has-text-centered">
        <div class="field">
          <label class="label">Unit Price</label>
          <div class="control has-text-centered">
            <input
              class="input"
              type="text"
              v-model="price"
              placeholder="units"
            />
          </div>
        </div>
      </div>
      <div class="column has-text-right">
        <div class="field">
          <label class="label">Price</label>
          <div class="control has-text-right">
            <strong>{{ price }}€</strong>
          </div>
        </div>
      </div>
    </div>
    <div class="columns has-text-right">
      <div class="column">
        <span class="tag">
          IVA: <strong>{{ iva }}%</strong>
        </span>
      </div>
    </div>
    <div class="columns">
      <div class="column has-text-right">
        <span>
          <strong></strong>
        </span>
      </div>
    </div>
    <div class="columns">
      <div class="column has-text-centered">
        <button class="button is-primary">
          Send
        </button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      units: 0,
      price: 10,
      iva: 10,
      errorMessage: null
    }
  }
}
</script>

<style lang="scss" scoped>
.img-pizza {
  width: 200px;
  height: auto;
}
</style>
