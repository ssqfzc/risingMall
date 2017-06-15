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
html{
  font-size: 16px;
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
  margin-top: 2.6rem;
}
.el-dialog--tiny{
  width: 100% !important;
}
.router-link-active{
  background: #20A0FF;
}
.el-message-box{
  width: 80% !important;
}
.el-message{
  top: 3rem !important;
}
.el-time-spinner__list{
  clear: both;
}
.el-time-spinner__list > li{
  float: left;
}
/*html {font-size:10px}*/
@media screen and (min-width:480px) and (max-width:639px) {
    html {
        font-size: 15px
    }
}
@media screen and (min-width:640px) and (max-width:719px) {
    html {
        font-size: 20px
    }
}
@media screen and (min-width:720px) and (max-width:749px) {
    html {
        font-size: 22.5px
    }
}
@media screen and (min-width:750px) and (max-width:799px) {
    html {
        font-size: 23.5px
    }
}
@media screen and (min-width:800px) and (max-width:959px) {
    html {
        font-size: 25px
    }
}
@media screen and (min-width:960px) and (max-width:1079px) {
    html {
        font-size: 30px
    }
}
@media screen and (min-width:1080px) {
    html {
        font-size: 32px
    }
}
</style>
