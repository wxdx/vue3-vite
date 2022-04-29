<template>
  <div class="layout">
    <div class="layout-top">
      <Header />
    </div>
    <div class="layout-bootom">
      <Menu class="layout-bootom-menu" />
      <Content class="layout-bootom-content" />
    </div>
  </div>
</template>

<script setup lang="ts">
import Menu from "./Menu/index.vue"
import Header from "./Header/index.vue"
import Content from "./Content/index.vue"
</script>
<style scoped lang="less">
.layout {
  display: flex;
  flex-direction: column;
  height: 100%;
  &-top {
    height: 80px;
  }
  &-bootom {
    flex: 1;
    display: flex;
    &-menu {
      width: 200px;
    }
    &-content {
      flex: 1;
    }
  }
}
</style>
