<template>
  <div id="app">
    <!-- <MyMonaco /> -->
    <!-- <calendarHeatmap /> -->
    <el-container>
      <el-header class="header-container">Header</el-header>
      <el-container>
        <el-aside width="200px">
            <Menu />
        </el-aside>
        <el-main>
          <router-view />
        </el-main>
      </el-container>
    </el-container>
  </div>
</template>
<script>
import MyMonaco from "./views/myMonaco";
import calendarHeatmap from "./views/calendarHeatmap";
import Menu from "@/components/menu";
export default {
  components: {
    MyMonaco,
    calendarHeatmap,
    Menu
  },
};
</script>
<style lang="scss">
* {
  margin: 0;
  padding: 0;
}
.header-container {
  background: #232940;
}
</style>
