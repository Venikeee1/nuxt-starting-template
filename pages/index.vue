<template>
  <div class="wrapper">
    <Header />
    <Footer />
  </div>
</template>

<script>
import Header from '@/components/header/Header.vue'
import Footer from '@/components/footer/Footer.vue'

export default {
  components: {
    Header,
    Footer
  }
}
</script>

<style lang="scss">

  .wrapper {
    min-height: 100vh;
    background: $dark-color;
  }
</style>

