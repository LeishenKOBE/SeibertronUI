<template>
  <button class="xr-button" @click="_click" :class="[xrButtonPrimary]"><slot></slot></button>
</template>
<script>
export default {
  name: "XrButton",
  data() {
    return {
      xrButtonPrimary:''
    };
  },
  methods: {
    _click(){
      this.$emit('click',function(){
        
      })
    }
  },
  props: ["type"],
  mounted(){
    if(this.type == 'primary'){
      this.xrButtonPrimary = 'xt-button-primary'
    }
  }
};
</script>
<style scoped lang='less' >
.xr-button {
  display: inline-block;
  border-radius: 3px;
  text-align: center;
  cursor: pointer;
  border: 1px solid #dcdfe6;
  width: 90px;
  height: 40px;
  color: #606266;
  font-size: 14px;
  white-space: nowrap;
  text-align: center;
  background: white;
  font-weight: 500;
  margin:20px;
}
.xr-button:hover {
  border: 1px solid rgb(64, 158, 255);
  color: rgb(64, 158, 255);
  font-weight: 500;
}
.xr-button:active {
  border: 1px solid rgb(64, 158, 255);
  color: rgb(64, 158, 255);
  font-weight: 500;
}

.xt-button-primary{
  display: inline-block;
  border-radius: 3px;
  text-align: center;
  cursor: pointer;
  border: none;
  width: 90px;
  height: 40px;
  color: white;
  font-size: 14px;
  white-space: nowrap;
  text-align: center;
  background: rgb(64, 158, 255);
  font-weight: 500;
}
.xt-button-primary:hover{
  color:white;
  background: rgba(64, 158, 255,.6);
  border:none;
}
.xt-button-primary:active{
  color:white;
  background: rgba(64, 158, 255,.6);
  border: none;
}
</style>
