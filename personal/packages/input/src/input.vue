<template>
  <input class="xr-input" />
</template>
<script>
export default {
  name: "XrInput"
};
</script>
<style scoped lang='less'>
.xr-input {
  width: 150px;
  padding: 0 15px;
  box-sizing: border-box;
  background-color: #fff;
  background-image: none;
  border-radius: 4px;
  border: 1px solid #dcdfe6;
  box-sizing: border-box;
  color: #606266;
  display: inline-block;
  font-size: inherit;
  height: 40px;
  line-height: 40px;
  outline: none;
}
.xr-input:focus{
    border:1px solid #606266;
}
</style>
