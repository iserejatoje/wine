<template>
  <div class='app'>
    <div class='app-inner'>
      <Header />
      <div class='wrapper'>
        <div class='container'>
          <Nuxt />
        </div>
      </div>
    </div>
    <Footer />
  </div>
</template>

<script lang='ts'>
import Vue from 'vue'

import Header from '~/components/Header.vue'
import Footer from '~/components/Footer.vue'

export default Vue.extend({
  components: { Footer, Header },
})

</script>
