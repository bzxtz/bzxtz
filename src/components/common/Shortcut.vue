<template>
<div class="shortcut">
  <div class="w">
    <!-- 左边模块 -->
    <div class='fl'>
  <ul >
    <li>XX商城欢迎您!</li>
      <li><a href="javascript:;">请登录</a></li>
             <li><a href="javascript:;" class='style-red'>免费注册</a></li>
  </ul>    </div>
  <!-- 右边模块 -->
  <div class="fr">
  <ul>
        <li><a href="">我的订单</a></li>
             <li class="spacer"></li>
               <li><a href="">我的商城</a>     <svg t="1628318965950" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="2554" width="32" height="32"><path d="M161.06066667 369.773c0-9.942 3.728-19.746 11.323-27.341 15.052-15.188 39.63-15.188 54.819 0l282.519 281.968 282.65799999-282.107c15.188-15.052 39.63-15.052 54.81900001 1e-8 15.188 15.188 15.052 39.63 0 54.81899999l-309.99900002 309.309c-15.188 15.052-39.63 15.052-54.68199997 0l-309.99900001-309.309c-7.732-7.595-11.461-17.398-11.461-27.341z" p-id="2555"></path></svg>
               <div class='drop-down-1'></div>
               </li>
            <li class="spacer"></li>
                  <li><a href="">商城会员</a></li>
                    <li class="spacer"></li>
                         <li class='style-red'><a href="">企业采购  </a>   <svg t="1628318965950" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="2554" width="32" height="32"><path d="M161.06066667 369.773c0-9.942 3.728-19.746 11.323-27.341 15.052-15.188 39.63-15.188 54.819 0l282.519 281.968 282.65799999-282.107c15.188-15.052 39.63-15.052 54.81900001 1e-8 15.188 15.188 15.052 39.63 0 54.81899999l-309.99900002 309.309c-15.188 15.052-39.63 15.052-54.68199997 0l-309.99900001-309.309c-7.732-7.595-11.461-17.398-11.461-27.341z" p-id="2555"></path></svg></li>
                           <li class="spacer"></li>
                          <li><a href="">客户服务 </a>    <svg t="1628318965950" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="2554" width="32" height="32"><path d="M161.06066667 369.773c0-9.942 3.728-19.746 11.323-27.341 15.052-15.188 39.63-15.188 54.819 0l282.519 281.968 282.65799999-282.107c15.188-15.052 39.63-15.052 54.81900001 1e-8 15.188 15.188 15.052 39.63 0 54.81899999l-309.99900002 309.309c-15.188 15.052-39.63 15.052-54.68199997 0l-309.99900001-309.309c-7.732-7.595-11.461-17.398-11.461-27.341z" p-id="2555"></path></svg></li>
                            <li class="spacer"></li>
                              <li><a href="">网址导航</a>     <svg t="1628318965950" class="icon" viewBox="0 0 1024 1024" version="1.1" xmlns="http://www.w3.org/2000/svg" p-id="2554" width="32" height="32"><path d="M161.06066667 369.773c0-9.942 3.728-19.746 11.323-27.341 15.052-15.188 39.63-15.188 54.819 0l282.519 281.968 282.65799999-282.107c15.188-15.052 39.63-15.052 54.81900001 1e-8 15.188 15.188 15.052 39.63 0 54.81899999l-309.99900002 309.309c-15.188 15.052-39.63 15.052-54.68199997 0l-309.99900001-309.309c-7.732-7.595-11.461-17.398-11.461-27.341z" p-id="2555"></path></svg></li>
  </ul>
  </div>
</div>
</div>
</template>

<script>
export default {
name:'Shortcut'
}
</script>

<style >
.shortcut{
  height: 31px;
  background-color: #e3e4e5;;  
    line-height: 31px;
}

.fl li{float: left;
padding:0 5px}
.fr li{float: left;
}
.fr svg{
  vertical-align: middle;
  height: 12px;
  width: 12px;
}
.spacer{
  margin:9px 30px;
  width: 1px;
  height: 12px;
	background-color: #666;  
}
.drop-down-1{
  position:absolute;
}
</style>