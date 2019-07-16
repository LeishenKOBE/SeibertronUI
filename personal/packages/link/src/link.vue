<template>
  <a href="https://www.baidu.com" target="view_window" class="xr-link">
    <slot>链接</slot>
  </a>
</template>
<script>
export default {
  name: "XrLink"
};
</script>
<style scoped lang='less'>
.xr-link {
  text-decoration: none;
  color: #606266;
  cursor: pointer;
  font-size: 14px;
  font-weight: 500;
  margin:0 10px;
}
.xr-link:hover {
    color:#409eff;
}
</style>
