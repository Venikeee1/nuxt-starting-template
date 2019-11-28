<template>
  <a
    href="/"
    class="app-logo"
  >
    <Logo class="main-logo" />
  </a>
</template>

<script>
import Logo from '@/components/svg/Logo.vue'

export default {
  name: 'AppLogo',
  components: {
    Logo
  }
}
</script>

<style lang="scss">
.main-logo {
  fill: #fff;
}
</style>

