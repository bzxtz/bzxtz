<template>
  <div class="footer clear-fix">
    <!-- 图标模块 -->
    <div class="mod-service">
      <div class="w">
        <ul>
          <li>
            <i></i>
            <h4>品类齐全，轻松购物</h4>
          </li>
          <li>
            <i></i>
            <h4>多仓直发，极速配送</h4>
          </li>
          <li>
            <i></i>
            <h4>正品行货，精致服务</h4>
          </li>
          <li>
            <i></i>
            <h4>天天低价，畅选无忧</h4>
          </li>
        </ul>
      </div>
    </div>
    <!-- 帮助模块 -->
    <div class="mod-help">
      <div class="w">
        <dl class="mod-help-item">
          <dt><h3>购物指南</h3></dt>
          <dd><a href="javascript:;">购物流程</a></dd>
          <dd><a href="javascript:;">会员介绍</a></dd>
          <dd><a href="javascript:;">生活旅行</a></dd>
          <dd><a href="javascript:;">常见问题</a></dd>
          <dd><a href="javascript:;">大家电</a></dd>
          <dd><a href="javascript:;">联系客服</a></dd>
        </dl>
        <dl class="mod-help-item">
          <dt><h3>配送方式</h3></dt>
          <dd><a href="javascript:;">上门自提</a></dd>
          <dd><a href="javascript:;">211限时达</a></dd>
          <dd><a href="javascript:;">配送服务查询</a></dd>
          <dd><a href="javascript:;">配送费收取标准</a></dd>
          <dd><a href="javascript:;">海外配送</a></dd>
        </dl>
        <dl class="mod-help-item">
          <dt><h3>支付方式</h3></dt>
          <dd><a href="javascript:;">货到付款</a></dd>
          <dd><a href="javascript:;">在线支付</a></dd>
          <dd><a href="javascript:;">分期付款</a></dd>
          <dd><a href="javascript:;">公司转账</a></dd>
        </dl>
        <dl class="mod-help-item">
          <dt><h3>售后服务</h3></dt>
          <dd><a href="javascript:;">售后政策</a></dd>
          <dd><a href="javascript:;">价格保护</a></dd>
          <dd><a href="javascript:;">退款说明</a></dd>
          <dd><a href="javascript:;">返修/退还货</a></dd>
          <dd><a href="javascript:;">取消订单</a></dd>
        </dl>
        <dl class="mod-help-item">
          <dt><h3>特色服务</h3></dt>
          <dd><a href="javascript:;">夺宝岛</a></dd>
          <dd><a href="javascript:;">延保服务</a></dd>
        </dl>
      </div>
    </div>
    <!-- 版权模块 -->
    <div class="mod-copyright clear-fix">
      <div class="w">
        <div class="mod-copyright-links">
          <ul>
            <li><a href="javascript:;">关于我们</a></li>
            <li class="mod-copyright-split"></li>
            <li><a href="javascript:;">联系我们</a></li>
            <li class="mod-copyright-split"></li>
            <li><a href="javascript:;">联系客服</a></li>
            <li class="mod-copyright-split"></li>
            <li><a href="javascript:;">商家入驻</a></li>
            <li class="mod-copyright-split"></li>
            <li><a href="javascript:;">营销中心</a></li>
            <li class="mod-copyright-split"></li>
            <li><a href="javascript:;">友情链接</a></li>
            <li class="mod-copyright-split"></li>
            <li><a href="javascript:;">销售联盟</a></li>
            <li class="mod-copyright-split"></li>
            <li><a href="javascript:;">English Site</a></li>
            <li class="mod-copyright-split"></li>
            <li><a href="javascript:;">Contact U</a></li>
          </ul>
        </div>
        <div class="mod_copyright_info">
          地址：北京市昌平区建材城西路金燕龙办公楼一层 邮编：100096
          电话：400-618-4000 传真：010-82935100 邮箱: zhanghj+itcast.cn <br />
          京ICP备08001421号京公网安备110108007702
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Footer",
  // 不能小写命名，要么a-b要么A-B要么Abc这样子
};
</script>

<style scoped>
.footer {
  margin-top: 10x;
  margin-bottom: 50px;
}
.mod-service {
  height: 103px;
  border-bottom: 1px solid #dedede;
}
.mod-service li {
  float: left;
  width: 25%;
  height: 103px;
  line-height: 103px;
}
.mod-service li i {
  float: left;
  width: 36px;
  height: 42px;
  margin-top: 30px;
}
.mod-service li:nth-child(1) i {
  background: url(~assets/img/footer-images.png) no-repeat;
  background-size: 113px 86.5px;
}
.mod-service li:nth-child(2) i {
  background: url(~assets/img/footer-images.png) no-repeat -38px 0;
  background-size: 113px 86.5px;
}
.mod-service li:nth-child(3) i {
  background: url(~assets/img/footer-images.png) no-repeat -76px 0;
  background-size: 113px 86.5px;
}
.mod-service li:nth-child(4) i {
  background: url(~assets/img/footer-images.png) no-repeat 0 -44px;
  background-size: 113px 86.5px;
}
.mod-help-item {
  float: left;
  margin-top: 20px;
  width: 20%;
  text-align: center;
  height: 200px;
}
.mod-help-item dd {
  height: 22px;
  line-height: 22px;
}
.mod-help .w {
  height: 200px;
  border-bottom: 1px solid #dedede;
}
.mod-copyright {
  height: 90px;
}
.mod-copyright-links ul {
  height: 23px;
  line-height: 18px;
}
.mod-copyright-links {
  margin: 0 auto;
  padding-left: 200px;
}

.mod-copyright-links li {
  float: left;
}
.mod-copyright-links .mod-copyright-split {
  margin: 3px 20px;
  width: 1px;
  height: 12px;
  background-color: #dedede;
}
.mod_copyright_info {
  margin-top: 25px;
  text-align: center;
  line-height: 18px;
  height: 40px;
}
</style>