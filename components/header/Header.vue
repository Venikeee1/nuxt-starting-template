<template>
  <header class="header">
    <div class="container">
      <div class="header__inner">
        <AppLogo />
        <Navigation />
        <Btn>Contact us</Btn>
      </div>
    </div>
  </header>
</template>

<script>
import AppLogo from '@/components/AppLogo.vue'
import Navigation from '@/components/navigation/Navigation.vue'
import Btn from '@/components/general/buttons/Btn.vue'

export default {
  name: 'Header',
  components: {
    AppLogo,
    Navigation,
    Btn
  }
}
</script>

<style lang="scss" scoped>

  .header {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    padding: 65px 0 30px;

    &__inner {
      display: flex;
      justify-content: space-between;
      align-items: center;
    }
  }

</style>
