<template>
  <div class="header">
    <el-button class="out" type="" @click="loginout">退出登录</el-button>
  </div>
</template>
<script>
export default {
  methods: {
    loginout() {
      this.$router.push('/loginIn');
    }
  }
};
</script>
<style>
.header {
  height: 60px;
  width: 100%;
  background-color: #efefef;
  display: flex;
  justify-content: flex-end;
  align-items: center;
}
.out {
  float: right;
  margin-right: 20px;
}
</style>


