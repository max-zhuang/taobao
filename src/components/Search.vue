<template>
  <div class="Search-box">
    <div class="img-box">
    <img src="../assets/taobao-logo.png" />
    </div>
    <div class="input-box">
      <el-input></el-input>
    </div>
  </div>
</template>

<script>
export default {
  name: "Search",
};
</script>

<style>
.Search-box {
  display: flex;
  flex-direction: row;
  margin: 10px;
}

.input-box {
  width: 800px;
  margin: 10px;
}
.img-box{
  width: 212px;
}

.el-input__inner {
  height: 36px !important;
 border-radius: 20px !important;
 border-color: rgb(255, 80, 0) !important;
}



</style>