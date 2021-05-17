<template>
  <header>
    <div class='header-left'>
      <NuxtLink class='header-home__link' to='/'><h1>WineShop</h1></NuxtLink>
    </div>
    <div class='header-nav'>
      <nav>
        <NuxtLink active-class='header-nav__item-active' to='/' exact class='header-nav__item'>Главная</NuxtLink>
        <NuxtLink no-prefetch active-class='header-nav__item-active' to='/catalog' class='header-nav__item'>Каталог</NuxtLink>
        <NuxtLink no-prefetch active-class='header-nav__item-active' to='/about' class='header-nav__item'>О нашей компании</NuxtLink>
        <NuxtLink no-prefetch active-class='header-nav__item-active' to='/cart' class='header-nav__item'>
          <svg height="24" viewBox="0 0 24 24" width="24" xmlns="http://www.w3.org/2000/svg"><circle cx="8" cy="21" fill="none" r="2" stroke="#fff" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"/><circle cx="20" cy="21" fill="none" r="2" stroke="#fff" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"/><path d="M5.67,6H23l-1.68,8.39a2,2,0,0,1-2,1.61H8.75a2,2,0,0,1-2-1.74L5.23,2.74A2,2,0,0,0,3.25,1H1" fill="none" stroke="#fff" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"/></svg><span class='cart-count'>2</span></NuxtLink>
      </nav>
    </div>
  </header>
</template>

<script lang='ts'>
import Vue from 'vue'

export default Vue.extend({})
</script>
