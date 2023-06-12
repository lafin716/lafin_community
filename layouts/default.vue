<template>
  <el-container>
    <el-header height="">
      <LCHeader></LCHeader>
    </el-header>
    <el-main>
      <nuxt />
    </el-main>
    <el-footer>Footer</el-footer>
  </el-container>
</template>

<script>
import LCHeader from '~/components/layouts/LCHeader.vue'

export default {
  components: {
    LCHeader,
  },
}
</script>

<style lang="scss" scoped></style>
