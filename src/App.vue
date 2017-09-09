<template>
  <div id="app" class="app">
    <v-header></v-header>
    <div class="tab">
      <div class="tab-item">
        <router-link to="/goods"><span>商品</span></router-link>
        </div>
      <div class="tab-item">
        <router-link to="/ratings"><span>评价</span></router-link>
      </div>
      <div class="tab-item">
        <router-link to="/seller"><span>商家</span></router-link>
      </div>
    </div>
    <router-view></router-view>
  </div>
</template>
<script>
  import top from './components/header/header.vue'
  export default {
    name: 'app',
    components:{
      "v-header":top
    }
  }
</script>
<style>
  .app .tab{
    display: flex;
    width: 100%;
    /* height: 400px; */
    line-height: 40px;
  }
  .tab .tab-item{
    flex: 1;
    text-align: center;
  }
  .tab-item  span{
    color: #333333
  }
</style>
