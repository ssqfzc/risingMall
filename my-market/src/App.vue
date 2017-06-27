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
.footer{
  position: fixed;
  bottom: 0;
  width: 100%;
  display: flex;
  justify-content: space-around;
  background-color: #fff;
  height:45px;
  line-height: 50px;
}

.mint-searchbar{
  background-color: #459ae9;
}

.mint-searchbar-cancel{
  display: none;
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
