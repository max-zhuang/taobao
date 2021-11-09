<template>
  <div class="secongimg"> 
    <img src="../assets/secondimg-picture1.png" class="picture"/>
    <img src="../assets/secondimg-picture2.png" class="picture"/>
  </div>
</template>

<script>
export default {
   nmae:"SecongImg"
}
</script>

<style>
.secongimg{
  display: flex;
  flex-direction: row;
  background-color:#ebebeb ;
  border-radius: 12px;
 
}
.picture{
  display: flex;
  border-radius: 12px;
  margin: 6px 6px 6px 3px;
  
}
</style>