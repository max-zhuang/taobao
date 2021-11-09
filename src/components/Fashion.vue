<template>
  <div class="fashion">
<BigImage/>
<Information/>
  </div>
</template>

<script>
import BigImage from "./BigImage.vue"
import Information from "./Information.vue"
/**
 * Bigimage组件
 * information组件
 */
export default {
  name:"Fashion",
  components:{
    BigImage,Information
  }

}
</script>

<style>
.fashion{
  display: flex;
  flex-direction: row;
}
</style>