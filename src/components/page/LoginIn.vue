<template>
  <div class="back">
    <div id="form">
    <el-form ref="form" :model="form" label-width="100px">
      <el-form-item label="帐号">
        <el-input v-model="form.name" placeholder="请输入您的帐号"></el-input>
      </el-form-item>
      <el-form-item label="密码">
        <el-input v-model="form.pwd" placeholder="请输入您的密码"></el-input>
      </el-form-item>
      <el-form-item>
        <el-button type="primary" @click="login">登录</el-button>
        <el-button type="" @click="reset">取消</el-button>
        <el-button type="success">注册</el-button>
      </el-form-item>
    </el-form>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      form: {
        name: 'admin',
        pwd: '123456'
      }
    };
  },
  methods: {
    login() {
      // if (
      //   this.$refs['form'].name === 'admin' &&
      //   this.$refs['form'].pwd === '123456'
      // ) {
      this.$router.push('/');
      // }
    },
    reset() {}
  }
};
</script>
<style>
.back {
  position: absolute;
  height: 100%;
  width: 100%;
  background: rgba(0, 0, 0, 0.1);
  background-size: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
}
#form {
  position: relative;
  width: 600px;
  height: 200px;
  background: rgb(255, 255, 255);
  right: 100px;
}
</style>


