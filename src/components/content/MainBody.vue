<template>
  <!-- 左侧导航栏 -->
  <div class="main-content clear-fix">
    <!-- 子盒子浮动，父盒子没高度就得清除浮动，不然影响布局 -->
    <div class="w">
      <div class="dropdown fl">
        <div class="dd">
          <ul>
            <li class="menu_item"><a href="#">家用电器</a></li>
            <li class="menu_item">
              <a href="list.html">手机</a> 、 <a href="#">数码</a> 、
              <a href="#">通信</a>
            </li>
            <li class="menu_item"><a href="#">电脑、办公</a></li>
            <li class="menu_item"><a href="#">家居、家具、家装、厨具</a></li>
            <li class="menu_item"><a href="#">男装、女装、童装、内衣</a></li>
            <li class="menu_item"><a href="#">个户化妆、清洁用品、宠物</a></li>
            <li class="menu_item"><a href="#">鞋靴、箱包、珠宝、奢侈品</a></li>
            <li class="menu_item"><a href="#">运动户外、钟表</a></li>
            <li class="menu_item"><a href="#">汽车、汽车用品</a></li>
            <li class="menu_item"><a href="#">母婴、玩具乐器</a></li>
            <li class="menu_item"><a href="#">食品、酒类、生鲜、特产</a></li>
            <li class="menu_item"><a href="#">医药保健</a></li>
            <li class="menu_item"><a href="#">图书、音像、电子书</a></li>
            <li class="menu_item"><a href="#">彩票、旅行、充值、票务</a></li>
            <li class="menu_item"><a href="#">理财、众筹、白条、保险</a></li>
          </ul>
        </div>
      </div>
      <!-- 右侧main制作 -->
      <!-- <element-ui轮播图> -->
      <div class="lunbo">
        <el-carousel :interval="5000" arrow="always">
          <el-carousel-item v-for="(item, index) in images" :key="index">
            <a href="javascript:;"><img :src="item" /></a>
          </el-carousel-item>
        </el-carousel>
      </div>
      <!-- 子盒子不适合浮动，就用个父盒子包起来，然后浮动即可 -->
      <!-- 快报模块 -->
      <div class="newsflash fr">
        <div class="news">
          <div class="news-hd">
            快报
            <a href="#">更多</a>
          </div>
          <div class="news-bd">
            <ul>
              <li><a href="#">【特惠】爆款耳机5折秒！</a></li>
              <li><a href="#">【特惠】母亲节，健康好礼低至5折！</a></li>
              <li><a href="#">【特惠】爆款耳机5折秒！</a></li>
              <li><a href="#">【特惠】9.9元洗100张照片！</a></li>
              <li><a href="#">【特惠】长虹智能空调立省1000</a></li>
            </ul>
          </div>
        </div>
        <div class="lifeservice">
          <ul>
            <li>
              <a href="#">
                <i class="service_ico"
                  ><img src="../../assets/img/a.png" alt=""
                /></i>
                <p>话费</p>
              </a>
            </li>
            <li>
              <a href="#">
                <i class="service_ico"
                  ><img src="../../assets/img/b.png" alt=""
                /></i>
                <p>机票</p>
              </a>
              <span class="hot"></span>
            </li>
            <li>
              <a href="#">
                <i class="service_ico"
                  ><img src="../../assets/img/c.png" alt=""
                /></i>
                <p>酒店</p>
              </a>
            </li>
            <li>
              <a href="#">
                <i class="service_ico"
                  ><img src="../../assets/img/d.png" alt=""
                /></i>
                <p>游戏</p>
              </a>
            </li>
            <li>
              <a href="#">
                <i class="service_ico"
                  ><img src="../../assets/img/e.png" alt=""
                /></i>
                <p>加油卡</p>
              </a>
            </li>
            <li>
              <a href="#">
                <i class="service_ico"
                  ><img src="../../assets/img/f.png" alt=""
                /></i>
                <p>火车票</p>
              </a>
            </li>
            <li>
              <a href="#">
                <i class="service_ico"
                  ><img src="../../assets/img/g.png" alt=""
                /></i>
                <p>众筹</p>
              </a>
            </li>
            <li>
              <a href="#">
                <i class="service_ico"
                  ><img src="../../assets/img/h.png" alt=""
                /></i>
                <p>机票</p>
              </a>
            </li>
            <li>
              <a href="#">
                <i class="service_ico"
                  ><img src="../../assets/img/i.png" alt=""
                /></i>
                <p>理财</p>
              </a>
            </li>
            <li>
              <a href="#">
                <i class="service_ico"
                  ><img src="../../assets/img/j.png" alt=""
                /></i>
                <p>电影票</p>
              </a>
            </li>
            <li>
              <a href="#">
                <i class="service_ico"
                  ><img src="../../assets/img/a.png" alt=""
                /></i>
                <p>企业购</p>
              </a>
            </li>
            <li>
              <a href="#">
                <i class="service_ico"
                  ><img src="../../assets/img/a.png" alt=""
                /></i>
                <p>礼品卡</p>
              </a>
            </li>
          </ul>
        </div>
        <div class="bargain">
          <img src="~assets/uploads/bargain.jpg" alt="" />
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "MainBody",
  data() {
    return {
      images: [
        require("../../assets/uploads/q(1).jpg"),
        require("assets/uploads/q(2).jpg"),
        require("assets/uploads/q(3).jpg"),
        require("assets/uploads/q(4).jpg"),
        require("assets/uploads/q(5).jpg"),
        require("assets/uploads/q(6).jpg"),
        //      原因：data 中 图片路径会被解析成字符串，所以使用时，找不到图片的路径
        // 解决方法： 通过require 引入，而require里无需加~
      ],
    };
  },
};
</script>
<style >
.lunbo {
  float: left;
}
.el-carousel,
.el-carousel--horizontal,
.el-carousel__container,
.el-carousel__item {
  width: 650px;
  height: 465px;
}
.el-carousel a {
  float: left;
  width: 100%;
  height: 100%;
}
.el-carousel img {
  width: 100%;
  height: 100%;
}
/*nav start*/

.dropdown {
  width: 209px;
  height: 45px;
  margin-right: 15px;
}
.dropdown .dd {
  height: 465px;
  background-color: #c81623;
  margin-top: 2px;
}

.menu_item:hover {
  background-color: #fff;
}
/*鼠标经过li 里面的 a变颜色*/
.menu_item:hover a {
  color: #c81623;
}

.menu_item {
  width: 100%;
  height: 31px;
  line-height: 31px;
  margin-left: 1px;
  padding: 0 10px;
  transition: all 0.5s;
}
.menu_item:hover {
  padding-left: 20px;
}
.menu_item a {
  font-size: 14px;
  color: #fff;
}

.navitems {
  margin-left: 10px;
}
.navitems li {
  float: left;
}
.navitems li a {
  display: block;
  height: 45px;
  padding: 0 25px;
  line-height: 45px;
  font-size: 16px;
}
/* news模块 */
.newsflash {
  margin-right: 30px;
  width: 249px;
}
.news {
  height: 163px;
  border: 1px solid #ccc;
}
.news-hd {
  height: 32px;
  /*dotted 点线  dashed  虚线*/
  border-bottom: 1px dotted #ccc;
  padding: 0 15px;
  font-size: 14px;
  line-height: 32px;
}
.news-hd a {
  float: right;
  font-size: 12px;
  font-family: "icomoon";
}
.news-bd {
  padding: 10px 0 0 15px;
}
.news-bd li {
  height: 23px;
}
.lifeservice {
  overflow: hidden;
  height: 208px;
  border: 1px solid #ccc;
  border-top: none;
}
.lifeservice ul {
  width: 252px;
}
.lifeservice li {
  position: relative;
  float: left;
  width: 62px;
  height: 70px;
  border-right: 1px solid #ccc;
  border-bottom: 1px solid #ccc;
}
.lifeservice li a {
  display: block;
  /* overflow: hidden; 解决i 引起的 外边距塌陷合并的问题*/
  overflow: hidden;
  height: 100%;
}
.lifeservice li p {
  text-align: center;
}

.service_ico {
  display: block;
  width: 24px;
  height: 24px;
  margin: 10px auto;
}
.service_ico img {
  width: 100%;
  height: 100%;
}
.bargain {
  height: 75px;
  margin-top: 5px;
}
</style>