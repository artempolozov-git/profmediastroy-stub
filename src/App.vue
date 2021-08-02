<template>
  <div id="app">
    <div id="app-content">
      <Home></Home>
    </div>
  </div>
</template>

<script>
import Home from './components/Home.vue'

export default {
  name: 'App',
  components: {
    Home
  }
}
</script>

<style>
  html, body {
    height: 100%;
    font-size: 16px;
  }
  body {
    margin: initial;
    font-family: RobotoCondensed;
  }
  #app {
    flex-direction: column;
    min-height: 100%;
  }
  @font-face {
    font-family: RobotoCondensed;
    src: url('./assets/RobotoCondensed-Bold.ttf');
    font-weight: bold;
    font-display: fallback;
  }
  @font-face {
    font-family: RobotoCondensed;
    src: url('./assets/RobotoCondensed-Regular.ttf');
    font-weight: normal;
  }
  #app-content {
    flex: 1 0 auto;
    max-width: 1920px;
    align-self: center;
    width: -webkit-fill-available;
  }
</style>
