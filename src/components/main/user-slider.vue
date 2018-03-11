<template>
  <div class="user-slider">
    <div class="slider__wrapper">
      <div class="slider__arrow"></div>
      <div class="slider__name">
        <p>Vladimir Holodkov</p>
      </div>
      <div class="slider__arrow"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'user-slider'
}
</script>

<style lang="scss" scoped>
.slider__wrapper {
  width: 80%;
  height: 80px;
  margin: 50px auto;
  background-color: darkgrey;

  .slider__name {
    display: flex;
    width: calc(100% - 80px);
    height: 100%;
    overflow-x: scroll;
    p {
      margin: auto;
    }
  }
}
</style>
