<template>
  <div class="home">
    <navigation-pager></navigation-pager>
    <footer>
      <mt-tabbar :fixed="true">
        <mt-tab-item>
          <img slot="icon" src="../img/home.gif">
          首页
        </mt-tab-item>
        <mt-tab-item>
          <img slot="icon" src="../img/car.gif">
          购物车
        </mt-tab-item>
        <mt-tab-item>
          <img slot="icon" src="../img/person.gif">
          个人中心
        </mt-tab-item>
      </mt-tabbar>
    </footer>
  </div>
</template>

<script>
import navigationPager from './nav/index'

export default {
  name: 'home',
  data () {
    return {
      tabContainerActive: 'tab-container-home',
      logintype: false
    }
  },
  methods: {
    linkToPath (path) {
      this.$router.push({ path: path })
    }
  },
  components: {
    navigationPager: navigationPager
  }
}
</script>
