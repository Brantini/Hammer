<template>
  <el-container>
    <el-header class="header">
      <span>工具集合</span>
    </el-header>
    <el-main class="main">
      <el-row>
        <el-menu
            class="menu"
            :default-active="activeIndex"
            mode="horizontal"
            @select="handleSelect"
        >
          <el-menu-item index="1">主页</el-menu-item>
          <el-sub-menu index="2">
            <template #title>问卷表</template>
            <el-menu-item index="2-1">所有问卷</el-menu-item>
            <el-menu-item index="2-2">新建问卷</el-menu-item>
            <el-menu-item index="2-3">导出问卷</el-menu-item>
          </el-sub-menu>
          <el-menu-item index="3">其他</el-menu-item>
          <el-menu-item index="4">公告</el-menu-item>
        </el-menu>
      </el-row>
    </el-main>
    <el-footer>Footer</el-footer>
  </el-container>
</template>

<script setup>

const activeIndex = '2-3'

const handleSelect = () => {
}
</script>

<style scoped>
.header {
  height: 4rem;
  background-color: #00a2dc;
  line-height: 4rem;
  font-size: 2rem;
  color: #fff;
}

.main {
  padding: 0;
  margin: 0;
}

.menu {
  width: 100%;
}

</style>