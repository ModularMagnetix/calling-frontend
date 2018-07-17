<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  width: 100vw;
  height: 100vh;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.button {
  width: 300px;
  height: 70px;
  background-color: rgba(0, 0, 0, 0.8);
  color: #dfdfdf;
  display: flex;
  cursor: pointer;
  text-transform: uppercase;
  p {
    margin: auto;
    font-size: 20px;
  }
}

.area {
  display: flex;
  p {
    margin: auto;
  }
}
</style>
