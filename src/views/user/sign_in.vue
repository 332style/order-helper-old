<template>
  <el-container class="container">
    <!-- <el-header>Header</el-header> -->
    <el-main>
      <div class="user-form">
        <el-input v-model="email" placeholder="请输入帳號"></el-input>
        <el-input
          placeholder="请输入密碼"
          v-model="password"
          show-password
        ></el-input>
        <el-button type="primary">登入</el-button>
      </div>
    </el-main>
  </el-container>
</template>
<style lang="scss">
.container {
  main {
    display: flex;
    justify-content: center;
    .user-form {
      max-width: 350px;
      border: 1px solid rgba(0, 0, 0, 0.6);
      border-radius: 5px;
      padding: 20px;
      .el-input {
        margin: 10px 0;
      }
      .el-button {
        margin-top: 10px;
      }
    }
  }
}
</style>
<script>
export default {
  data() {
    return {
      email: "",
      password: ""
    };
  }
};
</script>
