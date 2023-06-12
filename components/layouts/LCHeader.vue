<template>
  <div class="header">
    <div class="logo-wrap">
      <a href="/"><i class="el-icon-eleme"></i></a>
    </div>
    <div class="menu-wrap">
      <LCMenu />
      <div class="avatar-wrap">
        <LCAvatar />
      </div>
    </div>
  </div>
</template>

<script>
import LCMenu from './LCMenu.vue'
import LCAvatar from './LCAvatar.vue'

export default {
  components: { LCMenu, LCAvatar },
}
</script>

<style lang="scss" scoped>
.header {
  background-color: #545c64;
  color: #fff;
  text-align: center;
}
.logo-wrap {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  text-align: center;
  padding: 10px 30px;
  font-size: 50px;
}

.menu-wrap {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
}

.avatar-wrap {
  padding: 10px 30px;
}
</style>
