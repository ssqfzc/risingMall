<template>
  <div class="user">
    <div class="">
      user user user
    </div>
    <app-footer></app-footer>
  </div>
</template>

<script>
import appFooter from '../common/footer.vue'
export default {
  name: 'user',
  data () {
    return {
      msg: 'user'
    }
  },
  methods: {
    linkToPath (path) {
      this.$router.push({ path: path })
    }
  },
  components: {
    appFooter: appFooter
  }
}
</script>
<style scoped>

</style>
