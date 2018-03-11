<template>
  <div class="Main">
    <div class="sidebar">
        <user-slider></user-slider>
    </div>
    <sale-script></sale-script>
  </div>
</template>

<script>
export default {
  name: 'main',
  components: {
    'sale-script': () => import('./main/sale-script.vue'),
    'user-slider': () => import('./main/user-slider.vue')
  }
}
</script>

<style lang="scss" scoped>
  .Main {
    width: 100%;
    height: 100%;
  }

  .sidebar {
    width: 33vw;
    height: 100%;
    background-color: #605b9c;
    float: left;
  }
</style>
