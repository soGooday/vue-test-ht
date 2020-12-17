<template>
  <div>
      <el-button type="info" @click="loginOut">退出</el-button>
  </div>
</template>
<script>
export default {
    methods:{
        loginOut() {
            this.$router.push({path:'/login'});
            window.sessionStorage.removeItem('token');
        }
    }
}
</script>
<style lang="less" scoped>

</style>