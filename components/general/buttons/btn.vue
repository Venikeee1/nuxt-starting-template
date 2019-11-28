<template>
  <button class="btn">
    <slot></slot>
  </button>
</template>

<script>
export default {
  name: 'Btn'
}
</script>

<style lang="scss" scoped>
  .btn {
    background: none;
    border: 2px solid #fff;
    border-radius: 30px;
    font-size: 16px;
    color: #fff;
    padding: 3px 20px;
    line-height: 1.2;
  }

</style>
