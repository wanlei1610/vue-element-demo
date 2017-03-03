<template>
  <div id="app">
    <el-button type="primary">主要按钮</el-button>
    <el-button type="danger">主要按钮</el-button>
    <el-button type="info" icon='close'>主要按钮</el-button>
    <el-button type="success" icon='edit'>主要按钮</el-button>
    <el-button type="warning" icon='search'>主要按钮</el-button>
    <el-button type="text">文字按钮</el-button>
    <br>
    <span class='el-icon-delete'></span>
    <span class='el-icon-loading'></span>

    <el-row>
      <el-col :span="12">
        <div class="my-grid">AAA</div>
      </el-col>
      <el-col :span="12">
        <div class="my-grid">BBB</div>
      </el-col>
    </el-row>


    <el-row>
      <el-col :span="8">
        <div class="my-grid">
          <Date></Date>
        </div>
      </el-col>
      <el-col :span="8">
        <div class="my-grid">DDD</div>
      </el-col>
      <el-col :span="8">
        <div class="my-grid">EEE</div>
      </el-col>
    </el-row>
  </div>
</template>

<script>
  import Date from "./components/Date.vue"
export default {
  name: 'app',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
  components:{
      Date
  }
}
</script>

<style scoped lang="less">
  @color:yellowgreen;
  .height(@h){
    height:@h;
  }
  .my-grid{
    .height(50px);
    border:1px solid @color;
  }
</style>
