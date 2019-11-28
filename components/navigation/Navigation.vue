<template>
  <nav class="nav">
    <ul class="nav__list">
      <li
        v-for="navItem in navigation"
        :key="navItem.name"
        class="nav__item"
      >
        <a class="nav__link" href="">{{ navItem.name }}</a>
      </li>
    </ul>
  </nav>
</template>

<script>
export default {
  name: 'Navigation',
  data () {
    return {
      navigation: [
        {
          name: 'Services'
        },
        {
          name: 'Our works'
        },
        {
          name: 'Company'
        },
        {
          name: 'Careers'
        },
        {
          name: 'Blog'
        }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
.nav {
  color: #fff;
  &__list {
    display: flex;
    list-style: none;
  }

  &__item {
    padding: 5px 30px;
  }

  &__link {
    position: relative;
    display: inline-block;
    color: inherit;
    text-decoration: none;
    font-size: 16px;
    transition: 0.4s color;

    &::after {
      content: '';
      position: absolute;
      left: 0;
      bottom: -5px;
      height: 1px;
      width: 100%;
      background: $secondary-text-color;
      transition: transform 0.4s;
      transform: scaleX(0);
      transform-origin: 0 0;
    }

    &:hover {
      color: $secondary-text-color;

      &::after {
        transform: scaleX(1);
      }
    }
  }
}
</style>
