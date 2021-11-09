<template>
  <div class="tmall">
<Tmall/>
<Fashion/>
  </div>
</template>

<script>
import Tmall from "../components/Tmall.vue"
import Fashion from "../components/Fashion.vue"
/**
 * Tmall组件
 * Fashion组件
 */
export default {
  name:"ManyThings",
  components:{
    Tmall,Fashion
  }

}
</script>

<style>
.tmall{
  display: flex;
  flex-direction: column;
}
</style>