
<template>
    <div class="login">
      <el-form ref="form" :model="form" label-width="80px">
        <img src="../assets/avatar.jpg" alt="">
    <el-form-item label="用户名">
    <el-input v-model="form.username" placeholder="请输入用户名"></el-input>
    </el-form-item>
     <el-form-item label="密码">
    <el-input v-model="form.password" placeholder="请输入密码" type="password"></el-input>
    </el-form-item>
    <el-button type="primary">登录</el-button>
    <el-button>重置</el-button>
</el-form>
    </div>
</template>

<script>
export default {
  data() {
    return {
      form: {
        username: '',
        password: ''
      }
    }
  }
}
</script>

<style lang="less">
.login {
  height: 100%;
  background-color: #2b434c;
  overflow: hidden;
  .el-form {
    width: 400px;
    margin: 200px auto;
    background-color: #fff;
    padding: 75px 40px 40px 40px;
    border-radius: 20px;
    position: relative;
    img {
      position: absolute;
      top: -70px;
      left: 50%;
      transform: translateX(-50%);
      border-radius: 50%;
      border: 10px solid #fff;
    }
    .el-button {
      margin-left: 77px;
    }
  }
}
</style>
