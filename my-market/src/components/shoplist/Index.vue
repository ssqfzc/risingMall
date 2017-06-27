<template>
  <div class="shopList">
    <div class="">
      shopList
    </div>
    <!-- <app-footer></app-footer> -->
  </div>
</template>

<script>
// import appFooter from '../common/footer.vue'
export default {
  name: 'shopList',
  data () {
    return {
      msg: 'shopList'
    }
  },
  methods: {
    linkToPath (path) {
      this.$router.push({ path: path })
    }
  }
  // components: {
  //   appFooter: appFooter
  // }
}
</script>
<style scoped>

</style>
