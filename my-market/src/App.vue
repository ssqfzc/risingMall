<template>
  <div id="app">
    <!-- <img src="./assets/logo.png"> -->
    <router-view></router-view>
  </div>
</template>

<script>
export default {
  name: 'app'
}
</script>

<style>
.mint-searchbar{
  background-color: #459ae9;
}

.mint-searchbar-cancel{
  display: none;
}

.mint-tabbar > .mint-tab-item.is-selected{
  background-color: #fff;
}

html{
  font-size: 16px;
  background-color: #efeff4;
}

body{
  margin:0;
  padding: 0;
}

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
