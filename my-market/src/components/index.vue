<style scoped>
  .test{
    width: 100%;
    height: 300px;
    background: yellow;
  }
</style>
<template>
  <div class="home">
    <div class="test">
      <router-view></router-view>
    </div>
    <div class="footer">
      <div class=""><router-link :to='home'>{{this.home}}</router-link></div>
      <div class=""><router-link :to='shoplist'>{{this.cart}}</router-link></div>
      <div class=""><router-link :to='user'>{{this.user}}</router-link></div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'home',
  data () {
    return {
      home: '首页',
      cart: '购物车',
      user: '个人中心'
    }
  },
  methods: {
    linkToPath (path) {
      console.log(path)
      this.$router.push({ path: path })
    }
  }
}
</script>
