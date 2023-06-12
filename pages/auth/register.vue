<template>
  <el-card class="login-wrap">
    <div class="text item">
      <h2>회원가입</h2>

      <el-form
        :label-position="labelPosition"
        label-width="100px"
        :model="formLabelAlign"
      >
        <el-form-item label="Name">
          <el-input v-model="formLabelAlign.name"></el-input>
        </el-form-item>
        <el-form-item label="Activity zone">
          <el-input v-model="formLabelAlign.region"></el-input>
        </el-form-item>
        <el-form-item label="Activity form">
          <el-input v-model="formLabelAlign.type"></el-input>
        </el-form-item>
        <el-row class="sign-wrap">
          <NuxtLink to="/auth/findpassword">
            <el-link type="primary">비밀번호 찾기</el-link>
          </NuxtLink>
          <NuxtLink to="/auth/login">
            <el-link type="primary">이미 회원이신가요?</el-link>
          </NuxtLink>
        </el-row>
        <el-row>
          <el-button class="btn-wide" type="primary">로그인</el-button>
        </el-row>
      </el-form>
    </div>
  </el-card>
</template>

<script>
export default {
  layout: 'blank',
  data() {
    return {
      labelPosition: 'right',
      formLabelAlign: {
        name: '',
        region: '',
        type: '',
      },
    }
  },
}
</script>

<style lang="scss" scoped>
.login-wrap {
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  padding: 10px 30px;
}

.sign-wrap {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin: 20px 0;
}
</style>
