<template>
  <div class="main">
    <app-link v-show="$route.path !== '/home'"></app-link>
    <router-view></router-view>
  </div>
</template>

<script>
import AppLink from './Link'
export default {
    components:{AppLink}
};
</script>

<style scoped>
.el-breadcrumb {
  height: 10px;
  padding: 20px;
  border-radius: 4px;
  /* 投影 */
  box-shadow: 0 2px 12px 0 rgba(0, 0, 0, 0.1);
}
.line{
    border-left: 3px solid #31c17b;
    padding-left: 10px;
}
</style>