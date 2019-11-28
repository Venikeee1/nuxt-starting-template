<template>
    <ul class="social-media">
      <li
        v-for="socialItem in socialList"
        :key="socialItem"
        class="social-media__item"
      >
        <a :href="socialItem.link" class="social-media__link">
          <component :is="socialItem.name" class="social-media__icon"/>
        </a>
      </li>
    </ul>
</template>

<script>
import Instagram from '@/components/svg/Instagram'
import Linkedin from '@/components/svg/Linkedin'
import Facebook from '@/components/svg/Facebook'
import Twitter from '@/components/svg/Twitter'

const socialList = [
  {
    name: 'Instagram',
    link: '/'
  },
  {
    name: 'Linkedin',
    link: '/'
  },
  {
    name: 'Twitter',
    link: '/'
  },
  {
    name: 'Facebook',
    link: '/'
  }
]

export default {
  name: 'SocialMedia',
  components: {
    Instagram,
    Facebook,
    Twitter,
    Linkedin
  },
  data () {
    return {
      socialList
    }
  }
}
</script>

<style lang="scss" scoped>
  .social-media {
    display: flex;
    align-items: center;

    &__link {
      margin: 0 20px;

      &:last-child {
        margin-right: 0;
      }
    }

    &__icon {
      fill: #fff;
      width: 12px;
      height: 12px;
    }
  }
</style>
