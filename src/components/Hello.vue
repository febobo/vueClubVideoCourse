<template>
  <div class="video-list">
    <el-row :gutter="15">
      <el-col :span="6" v-for="i in [1,2,3,4,5,6,9,91]">
        <div class="course-description">
          <div class="image">
            <img src="https://a1.jikexueyuan.com/home/201611/03/fae6/581ae23c05942.jpg" alt="">
          </div>
          <div class="title">
            腾讯云产品 - 游戏云
          </div>
          <div class="course-info">
            <span>
              <i class="el-icon-time"></i>
              76分钟
            </span>
            <span>
              <i>4699</i>人学习
            </span>
          </div>
        </div>
      </el-col>
    </el-row>
  </div>
</template>

<script>
export default {
  name: 'hello',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App',
      currentDate: 'Welcome'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="less">
  .video-list{
    padding:15px 0px;
  }
  .el-row {
    margin-bottom: 20px;
    &:last-child {
      margin-bottom: 0;
    }
  }
  .bg-purple-dark {
    background: #99a9bf;
  }
  .bg-purple {
    background: #d3dce6;
  }
  .bg-purple-light {
    background: #e5e9f2;
  }
  .grid-content {
    border-radius: 4px;
    min-height: 36px;
  }
  .row-bg {
    padding: 10px 0;
    background-color: #f9fafc;
  }
  .course-description{
    position: relative;
    height: 210px;
    background: #fff;
    margin-bottom: 15px;
    .image{
      height: 152px;
      overflow: hidden;
    }
    img{
      width: 100%;
    }
    .title{
      text-align: left;
      padding: 8px;
      padding-bottom: 0;
    }
    .course-info{
      display: flex;
      width: 100%;
      justify-content: space-between;
      align-items: center;
      position: absolute;
      bottom: 0;
      height: 36px;
      font-size: 12px;
      padding:0 8px;
    }
  }
</style>
