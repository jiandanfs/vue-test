<template>
  <div class="wrap head">
    <input type="text" placeholder="请输入添加内容">
  </div>
</template>

<script>
export default {
  name: 'MyHeader',
  
}
</script>

<style scoped>
.head {
  height: 30px;
  padding: 5px;
  box-sizing: border-box;
}
input {
  padding: 0;
  height: 20px;
  border: none;
  outline: none;
  font-size: 14px;
}

</style>