<template>
  <div class="header">
    <el-menu theme="dark" :default-active="activeIndex" class="header-wrap" mode="horizontal" @select="handleSelect">
      <h2 class="logo">
        <img src="../assets/logo.png" alt="" >
        Vue中文社区视频课程
      </h2>
      <div class="nav">
        <el-menu-item index="2"><a href="https://www.ele.me" target="_blank">订单管理</a></el-menu-item>
        <el-submenu index="3">
          <template slot="title">设置</template>
          <el-menu-item index="2-1">选项1</el-menu-item>
          <el-menu-item index="2-2">选项2</el-menu-item>
          <el-menu-item index="2-3">选项3</el-menu-item>
        </el-submenu>
      </div>
    </el-menu>
  </div>
</template>

<script>
  export default {
    name: 'header',
    data () {
      return {
        activeIndex: '1',
      };
    }
  }
</script>


<style media="screen">
  .header{
    background: #324157;
    color: #fff;
  }
  .header-wrap{
    width: 1200px;
    margin: 0 auto !important;
  }
  .nav{
    float: right;
  }
  .logo{
    height: 60px;
    line-height: 60px;
    float: left;
    display: flex;
    align-items: center;
    font-size: 16px;
  }
  .logo img{
    height: 45px;
    width: 45px;
  }
</style>
