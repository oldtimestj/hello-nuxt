<template>
  <div>
    <h2>用户列表</h2>
    <nuxt-link to="/users">嵌套首页</nuxt-link>
    <nuxt-link to="/users/profile">嵌套详情</nuxt-link>
    <nuxt />
  </div>
</template>

<script>
  export default {
    name: 'User'
  }
</script>

<style scoped>

</style>
