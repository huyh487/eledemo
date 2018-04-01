<template>
  <div id="app">
    <header-self></header-self>
    <div class="tab">
      <div class="tab-item">
        <router-link to="/goods">商品</router-link>
      </div>
      <div class="tab-item">
        <router-link to="/rating">评论</router-link>
      </div>
      <div class="tab-item">
        <router-link to="/seller">商家</router-link>
      </div>
    </div>
    <div class="content">
      i am content origin.
    </div>

    <router-view></router-view>
  </div>
</template>
<script>
import header from '@/components/header/header.vue'
export default {
  components: {
    HeaderSelf: header
  }
}
</script>
<style>
.tab{
     display:flex;
      width:100%;
      height:40px;
      line-heigth:40px;
    }
      .tab-item{
        flex:1;
        text-align:center;
      }
</style>
