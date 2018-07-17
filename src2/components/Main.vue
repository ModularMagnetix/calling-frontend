<template>
  <!--
  <div class="Main">
    <div class="control-center">
      <div class="button"></div>
    </div>
    <div class="sidebar">
      <user-slider></user-slider>
      <tags-area></tags-area>
      <status></status>
    </div>
    <sale-script></sale-script>
  </div>
  -->
  <div class="main">
    <div class="control-center">
      <div class="button">
        <p>
          Перерыв
        </p>
      </div>
      <div class="time area">
        <p>
          {{ time }}
        </p>
      </div>
      <div class="icon-wrapper">
        <div class="icon">
          <img src="../assets/images/universal-access.svg">
        </div>
        <div class="icon">
          <img src="../assets/images/microoff.svg">
        </div>
        <div class="icon">
          <img src="../assets/images/profile.svg">
        </div>
        <div class="icon">
          <img src="../assets/images/shutdown.svg">
        </div>
      </div>
    </div>
    <div class="sidebar">
      <user-slider></user-slider>
      <tags-area></tags-area>
      <status></status>
    </div>
  </div>
</template>

<script>
export default {
  name: 'main',
  components: {
    'sale-script': () => import('./main/sale-script.vue'),
    'user-slider': () => import('./main/user-slider.vue'),
    'tags-area': () => import('./main/tags-area.vue'),
    'status': () => import('./main/status.vue')
  },
  computed: {
    time: function () {
      let date = new Date()
      return date.getHours() + ':' + date.getMinutes()
    }
  }
}
</script>

<style lang="scss" scoped>
  .main {
    width: 100vw;
    height: 100vh;
    background: linear-gradient(45deg, #EECFBA, #C5DDE8);
  }

  .control-center {
    width: 100%;
    height: 100px;
    background-color: rgba(0, 0, 0, 0.5);
    padding: 15px;
    display: flex;
    justify-content: space-between;

    .time {
      p {
        color: #dfdfdf;
        font-size: 30px;
      }
    }

    .icon-wrapper {
      height: 70px;
      width: 300px;
      display: flex;
      justify-content: space-between;

      .icon {
        cursor: pointer;
        img {
          height: 70px;
          width: 70px;
        }
      }
    }
  }

  .sidebar {
    width: 30vw;
    height: calc(100% - 100px);
    background-color: rgba(0, 0, 0, 0.5);
    padding-top: 80px;
  }
</style>
