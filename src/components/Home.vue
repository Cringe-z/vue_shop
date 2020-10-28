<template>
  <el-button type="info" @click="logout">退出</el-button>
</template>

<script>
export default {
  data() {
    return {};
  },
  methods: {
    logout() {
      window.sessionStorage.removeItem('token');
      this.$router.push('/login');
    },
  },
};
</script>

<style lang="less" scoped></style>
