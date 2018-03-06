<template>
  <div class="Main">
    <sale-script></sale-script>
  </div>
</template>

<script>
export default {
  name: 'main',
  components: {
    'sale-script': () => import('./main/sale-script.vue')
  }
}
</script>

<style lang="scss" scoped>

</style>
