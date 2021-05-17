<template>
  <div class='playground'>
    <div class='page-title_large'>Немного про винишко.<br/>Технологии &mdash; NuxtJs, Vue, NodeJs</div>
    <NuxtLink to='/catalog' class='base-link catalog-link'>В каталог <svg fill='#fff' width="24" height="24" xmlns="http://www.w3.org/2000/svg" fill-rule="evenodd" clip-rule="evenodd"><path d="M21.883 12l-7.527 6.235.644.765 9-7.521-9-7.479-.645.764 7.529 6.236h-21.884v1h21.883z"/></svg></NuxtLink>
  </div>
</template>

<script lang='ts'>
import Vue from 'vue'

export default Vue.extend({
  head() {
    return {
      title: 'Главная - WineShop'
    }
  }
})
</script>
