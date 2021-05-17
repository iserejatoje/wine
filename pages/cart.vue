<template>
  <div>
    <div class='page-title'>Корзина</div>
      {{ getName }}
  </div>
</template>

<script lang='ts'>
import Vue from 'vue'

export default Vue.extend({
  head() {
    return {
      title: 'Корзина - WineShop'
    }
  },
  computed: {
    getName () {
      return this.$store.getters['products/getName']
    }
  }
})
</script>
