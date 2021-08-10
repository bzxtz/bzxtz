<template>
  <!-- header模块 -->
  <div class="header">
    <div class="w">
      <div class="logo"><a href="javascript:;"></a></div>
      <div class="search-m">
        <!-- 搜索框 -->
        <div class="search-box">
          <input
            type="text"
            placeholder="请输入搜索内容 "
            class="search-input"
          />
          <button class="search-icon">搜索</button>
        </div>
        <!-- 购物车 -->
        <div class="shopcar">
          <a href="javascript:;">我的购物车</a>
        </div>
      </div>
      <!-- hotwords -->
      <div id="hotwords">
        <a href="javascript:;" class="style-red">家电秒杀</a>
        <a href="javascript:;">家装建材</a>
        <a href="javascript:;">食品饮料</a>
        <a href="javascript:;">健康好物</a>
        <a href="javascript:;">二手平板</a>
        <a href="javascript:;">笔记本</a>
        <a href="javascript:;">大屏电视</a>
      </div>
      <!-- nav-item -->
      <div class="nav-item">
        <ul class="fl">
          <li><a href="javascript:;">服装城</a></li>
          <li><a href="javascript:;">美妆馆</a></li>
          <li><a href="javascript:;">全球购</a></li>
          <li><a href="javascript:;">闪购</a></li>
          <li><a href="javascript:;">团购</a></li>
          <li><a href="javascript:;">拍卖</a></li>
          <li><a href="javascript:;">有趣</a></li>
          <li><a href="javascript:;">会员</a></li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style>
.w {
  position: relative;
}
.header {
  background-color: #fff;
}
.logo {
  width: 190px;
  height: 141px;
}
.logo a {
  display: block;
  margin-top: 3px;
  width: 190px;
  height: 141px;
  background: url("~@/assets/img/sprite@2x.png") no-repeat 0 21px;
  /* 写css时插入图片如果要用别名要加上~，切记，其他时候可以不用 */
  background-size: 190px 160px;
}
.search-m {
  position: absolute;
  z-index: 20;
  top: 0px;
  left: 0px;
  width: 100%;
  height: 60px;
}
.search-box {
  position: absolute;
  top: 26px;
  left: 230px;
  height: 34px;
  width: 490px;
  border: 2px solid red;
}
.shopcar {
  position: absolute;
  top: 26px;
  right: 40px;
  width: 132px;
  height: 35px;
  line-height: 35px;
  border: 1px solid #ccc;
  background: url("~assets/fonts/gouwuche.png") no-repeat 15px;
  background-size: 20px 20px;
}
.shopcar:hover {
  border: 1px solid red;
}
.shopcar a {
  display: inline-block;
  position: relative;
  margin-left: 47px;
  color: red;
}
.shopcar a::before {
  content: "0";
  position: absolute;
  top: 0px;
  left: -14px;
  width: 14px;
  height: 14px;
  line-height: 14px;
  text-align: center;
  background-color: rgb(223, 13, 118);
  border-radius: 6px 6px 6px 0;
  color: #fff;
}
.search-input {
  padding-left: 20px;
  height: 30px;
  width: 430px;
  font-size: 12px;
}
.search-icon {
  background-color: red;
  width: 56px;
  height: 30px;
  line-height: 30px;
  float: right;
  color: #fff;
  text-align: center;
}
#hotwords {
  position: absolute;
  left: 230px;
  top: 60px;
  width: 480px;
}
#hotwords a {
  display: inline-block;
  height: 30px;
  line-height: 30px;
  margin: 0 7px;
}
.nav-item {
  position: absolute;
  left: 230px;
  top: 100px;
}
.nav-item a {
  float: left;
  padding: 0 10px;
  height: 25px;
  line-height: 25px;
  font-size: 16px;
}
</style>