<template>


  <div class="login-box" id="app" >
    <el-row>
      <el-col :span="8">
        <el-input id="name"  v-model="username" placeholder="请输入帐号">
          <template slot="prepend">帐号</template>
        </el-input>
      </el-col>
    </el-row>
    <el-row>
      <el-col :span="8">
        <el-input id="password" v-model="password" type="password" placeholder="请输入密码">
          <template slot="prepend">密码</template>
        </el-input>
      </el-col>
    </el-row>
    <el-row>
      <el-col :span="8">
        <el-button id="login" v-on:click="check" style="width:100%" type="primary">登录</el-button>
      </el-col>
    </el-row>
  </div>

</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      username : '123456',
      msg: 'Welcome to Your Vue.js App'
    }
  },
  methods:{
    check(){
      alert(0)
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
