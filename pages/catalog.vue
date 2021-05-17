<template>
  <div>
    <div class='page-title'>Винная карта</div>

    <div class='catalog'>
      <NuxtLink to='' class='catalog-item' v-for='(wine, index) of wines' :key='wine.id'>
        <div class='catalog-item_image'>
          <img width='250' height='300' loading='lazy' :src="require(`~/assets/wines/${wine.picture}`)" alt=''>
        </div>
        <div class='catalog-item_information'>
          <div class='catalog-item_title'>{{ wine.name }}</div>
          <div class='catalog-item_spec'>
            <span>Страна: {{ wine.country }}</span>
            <span>Регион: {{ wine.region }}</span>
            <span>Год: {{ wine.year }}</span>
          </div>
        </div>
      </NuxtLink>
    </div>
  </div>
</template>

<script lang='ts'>
import Vue from 'vue'

export default Vue.extend({
  head() {
    return {
      title: 'Винная карта - WineShop'
    }
  },
  data: () => ({
    wines: []
  }),
  async mounted() {
    await this.$axios.$get('https://raw.githubusercontent.com/hollyschinsky/angular-cellar-basic/master/wines/wines.json').then(response => {
      this.wines = response
    })
  }
})
</script>

<style lang='scss' scoped src='assets/scss/_catalog.scss'></style>
