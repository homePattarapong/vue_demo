<template>
  <div>
    

    <ul>
      <li><router-link to="/">Home</router-link></li>
      <li><router-link to="/demo1">Demo1</router-link></li>
      <li><router-link to="/demo2">Demo2</router-link></li>
      <li><router-link to="/demo3">Demo3</router-link></li>
    </ul>

    <router-view></router-view>
    <span class="title">123</span>
  </div>
</template>

<script>
export default {
  name:"app",
 
}
</script>

<style scoped>
  ul{
    margin:0;
    padding:0;
  }
  li{
    display:inline;
    margin-right:8px;
  }
  .title{
    font-size: 30px;
  }
</style>