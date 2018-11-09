<template>
  <div class="left">
    <el-menu  :default-active="onRoutes" background-color="#324157" text-color="#bfcbd9" active-text-color="#20a0ff" unique-opened router>
    </el-menu>
  </div>
</template>
<script>
export default {
  computed: {
    onRoutes() {
      return this.$route.path.replace('/', '');
    }
  }
};
</script>

