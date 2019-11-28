<template>
  <footer class="footer">
    <div class="container">
      <div class="footer__inner">
        <AppLogo />
        <Navigation />
        <SocialMediaList />
      </div>
    </div>
  </footer>
</template>

<script>
import AppLogo from '@/components/AppLogo.vue'
import Navigation from '@/components/navigation/Navigation.vue'
import SocialMediaList from '@/components/footer/SocialMedia.vue'

export default {
  name: 'Header',
  components: {
    AppLogo,
    Navigation,
    SocialMediaList
  }
}
</script>

<style lang="scss" scoped>

  .footer {
    padding: 30px 0 60px;

    &__inner {
      display: flex;
      justify-content: space-between;
      align-items: center;
    }
  }

</style>
