<template>
  <div>
    <el-col :span="12">
      <el-menu
        default-active="2"
        class="el-menu-vertical-demo"
        background-color="#545c64"
        text-color="#fff"
        active-text-color="#ffd04b"
      >
        <el-submenu index="/home">
          <template slot="title">
            <i class="el-icon-location"></i>
            <span>element-ui 相关</span>
          </template>
          <el-menu-item-group>
            <el-menu-item index="1-1">redio 点击取消</el-menu-item>
            <el-menu-item index="1-2">选项2</el-menu-item>
          </el-menu-item-group>
        </el-submenu>
        <el-menu-item index="2">
          <i class="el-icon-menu"></i>
          <span slot="title">导航二</span>
        </el-menu-item>
        <el-menu-item index="3" disabled>
          <i class="el-icon-document"></i>
          <span slot="title">导航三</span>
        </el-menu-item>
        <el-menu-item index="4">
          <i class="el-icon-setting"></i>
          <span slot="title">导航四</span>
        </el-menu-item>
      </el-menu>
    </el-col>
  </div>
</template>
<script>
export default {};
</script>
<style lang="scss">
.el-menu-vertical-demo {
  width: 200px;
  box-sizing: border-box;
}
</style>