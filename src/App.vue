<template>
  <div id="app">
    <Header></Header>
    <div class="main">
      <router-view></router-view>
    </div>
  </div>
</template>

<script>
import Header from './components/Header'
export default {
  name: 'app',
  components: { Header }
}
</script>

<style lang="less">
.main{
  width: 1200px;
  margin:0 auto;
}
body{
  background: #e6e6e6;
}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  // text-align: center;
  color: #2c3e50;
}

body,li,h1,h2,h3,h4,h5,a,p,div,img{
  margin: 0;
  padding: 0;
  list-style: none;
  box-sizing: border-box;
}
</style>
