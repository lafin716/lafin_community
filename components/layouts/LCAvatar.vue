<template>
  <el-dropdown>
    <el-avatar size="medium" :src="avatarUrl"></el-avatar>
    <el-dropdown-menu slot="dropdown">
      <el-dropdown-item>Action 1</el-dropdown-item>
      <el-dropdown-item>Action 2</el-dropdown-item>
      <el-dropdown-item>Action 3</el-dropdown-item>
      <el-dropdown-item>Action 4</el-dropdown-item>
      <el-dropdown-item>Action 5</el-dropdown-item>
    </el-dropdown-menu>
  </el-dropdown>
</template>

<script>
export default {
  data() {
    return {
      avatarUrl: 'https://avatars3.githubusercontent.com/u/17571969?s=460&v=4',
    }
  },
}
</script>

<style lang="scss" scoped></style>
