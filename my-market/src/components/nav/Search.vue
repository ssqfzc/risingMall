<template>
  <div id="navSearch">
    <!-- <img src="./assets/logo.png"> -->
    <router-view></router-view>
    <div class="footer">
      <div class="" @click="linkToPath('home')">首页</div>
      <div class="" @click="linkToPath('shoplist')">购物车</div>
      <div class="" @click="linkToPath('user')">个人中心</div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'navSearch'
}
</script>

<style>

</style>
