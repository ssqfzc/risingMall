<template>
  <div id="navigation">
    <div class="nav-search">
      <mt-search placeholder="搜索"></mt-search>
    </div>
    <div class="nav-body">

      <!-- swipe轮播图 -->
      <mt-swipe :auto="4000" class="nav-swipe" :prevent="true">
        <mt-swipe-item><img src="../../img/1.jpg"  class="nav-swipe-img"/></mt-swipe-item>
        <mt-swipe-item><img src="../../img/2.jpg" class="nav-swipe-img"/></mt-swipe-item>
        <mt-swipe-item><img src="../../img/3.jpg" class="nav-swipe-img"/></mt-swipe-item>
      </mt-swipe>

      <!-- 分类 -->
      <div>
        <div class="nav-classify" v-for="item in classifys">
          <div class="nav-float-left" v-for="goods in item">{{goods}}</div>
        </div>
      </div>

      <!-- 推荐商品  -->
      <div class="nav-recommend-goods">
        <div class="nav-goods-row">
          <div class="nav-goods-col" @click="aa()">
            <img src="../../img/goods_1.jpg" width="100%" height="150px"/>
            <div class="nav-goods-color-title">美少女战士1</div>
            <div class="nav-text-left nav-goods-col-intro">¥99</div>
            <div class="nav-goods-col-intro">
              <div class="nav-float-left">¥79</div>
              <div class="nav-float-right">3111已买</div>
            </div>
          </div>
          <div class="nav-goods-col">
            <img src="../../img/goods_2.jpg" width="100%" height="150px"/>
            <div class="nav-goods-color-title">美少女战士2</div>
            <div class="nav-text-left nav-goods-col-intro">¥99</div>
            <div class="nav-goods-col-intro">
              <div class="nav-float-left">¥79</div>
              <div class="nav-float-right">3111已买</div>
            </div>
          </div>
        </div>
        <div class="nav-goods-row">
          <div class="nav-goods-col">
            <img src="../../img/goods_1.jpg" width="100%" height="150px"/>
            <div class="nav-goods-color-title">美少女战士3</div>
            <div class="nav-text-left nav-goods-col-intro">¥99</div>
            <div class="nav-goods-col-intro">
              <div class="nav-float-left">¥79</div>
              <div class="nav-float-right">3111已买</div>
            </div>
          </div>
          <div class="nav-goods-col">
            <img src="../../img/goods_2.jpg" width="100%" height="150px"/>
            <div class="nav-goods-color-title">美少女战士4</div>
            <div class="nav-text-left nav-goods-col-intro">¥99</div>
            <div class="nav-goods-col-intro">
              <div class="nav-float-left">¥79</div>
              <div class="nav-float-right">3111已买</div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'navigation',
  data () {
    return {
      classifys: [
        [
          '保健食品',
          'QS食品',
          '外用产品'
        ],
        [
          '一类医疗器械',
          '二类医疗器械',
          '计生用品'
        ]
      ],
      result: [
        'a', 'aw', 'aa', 'ab', 'ac', 'ae', 'af', 'ap', 'an', 'a', 'aw', 'aa', 'ab', 'ac', 'ae', 'af', 'ap', 'an'
      ]
    }
  },
  method: {
    aa () {
      console.log('aa')
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.nav-recommend-goods{
  margin-bottom: 65px;
}

.nav-float-left{
  float:left;
}

.nav-float-right{
  float: right;
}

.nav-swipe-img{
  height:180px;
}

.nav-search{
  position:fixed;
  top:0px;
  width: 100%;
  height:52px;
  z-index:2;
}

.mint-search{
  height:52px;
}

.nav-body{
  margin-top:52px;
  width: 100%;
  height: 180px;
  z-index:1;
}

.nav-classify{
  display: flex;
  padding: 0 10px;
  justify-content: space-around;
  text-align: center;
  margin: 15px 0;
}

.nav-classify div{
  width: 30%;
  background-color:#459ae9;
  border-radius: 6px;
  color: #fff;
  padding: 3px;
  height: 50px;
  line-height: 50px;
}

.nav-goods-row{
  display: flex;
  justify-content: space-around;
  text-align: center;
  margin-bottom: 10px;
}

.nav-goods-col{
  background-color: #fff;
  width: 100%;
  margin:0 10px;
  padding: 10px;
  color:#353535;
}

.nav-goods-col-intro{
  margin-top:12px;
}

.nav-text-left{
  text-align: left;;
}

.nav-goods-color-title{
  font-size: 14pt;
}
</style>
