<template>
  <div id="nav">
    <!-- <router-link to="/">Home</router-link> | -->
  </div>
  <router-view/>
</template>
<script>

import Home from 'views/Home'
export default{
  components:Home
}
</script>
<style>
@import 'assets/css/base.css';
@import 'assets/css/common.css';
/* 分号不能省 */
</style>
