<template>
  <div class="">
    <div class="course-header">
      <h2>腾讯云产品 - 游戏云</h2>
      <div class="course-tag">
        <el-tag type="primary" v-for="item in ['JS','Node','入门级']">{{item}}</el-tag>
      </div>
      <div class="course-progress">
        <span>当前进度：</span>
        <div class="progress">
          <el-progress :text-inside="true" :stroke-width="18" :percentage="100" status="success" ></el-progress>
        </div>
      </div>
      <div class="course-info">
        <p>⏰  课时：<span>59</span> 分钟</p>
        <p>🚀  目标：<span>一个人用javascript实现小程序登录和支付前后端功能</span></p>
        <p>🙇‍  适合对象：<span>有javascript基础，了解小程序基本代码结构，了解node的基本使用，对实现登录和支付感兴趣的同学。</span></p>
        <p>🎓  主讲老师：<span>刘焱旺</span></p>
      </div>
    </div>
    <div class="course-main">
      <video width="100%" height="100%" controls>
        <source src="http://ooaa8syjw.bkt.clouddn.com/001.mp4" type="video/mp4">
        <object data="http://ooaa8syjw.bkt.clouddn.com/001.mp4" width="100%" height="100%">
          <embed src="movie.swf" width="100%" height="100%">
        </object>
      </video>
    </div>
    <div class="course-desc">
      <h3>📚️  课程内容：</h3>
      <p class="desc-info">
      本课程主要讲解案例《GetWeApp金盆洗脚城》的设计思路和代码分析，实现了用户登录和支付的功能
      </p>
      <h4>具体内容包括：</h4>
      <ul>
        <li>课程目标设定</li>
        <li>知识点概述</li>
        <li>开发规划分析</li>
        <li>api设计思路</li>
        <li>前端开发源码分析</li>
        <li>服务端开发源码分析</li>
      </ul>
      <h4>
        应用截图&源码下载:<br>
        <a href="#">https://www.getweapp.com/project?projectId=5883a2f152e1e8733dc567e0</a>
      </h4>
    </div>
  </div>
</template>

<script>
  // import { Progress, Tag } from 'element-ui'
  export default {
    name: 'header',
    data () {
      return {
        activeIndex: '1',
      };
    }
  }
</script>


<style lang="less">
  .course-header{
    text-align: left;
    margin:15px 0;
    .course-tag span{
      margin-right: 10px;
    }
    >* {
      margin-bottom: 8px;
    }
    .course-progress{
      .progress{
        display: inline-block;
        width: 300px;
      }
    }
  }
  .course-main{
    height: 640px;
    overflow: hidden;
    background: #000;

  }
  .course-desc{
    margin:30px 0;
    .desc-info{
      margin-bottom: 16px;
    }
  }
</style>
