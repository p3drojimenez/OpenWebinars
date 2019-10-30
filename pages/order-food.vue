<template>
  <div>
    <a v-bind:href="url">Google</a>
  </div>
</template>

<script>
export default {
  data() {
    return {
      url: 'https://google.es'
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
