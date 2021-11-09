<template>
  <div class="show-box">
    <TaoBaoMarket />
    <ManyThings />
  </div>
</template>

<script>
import ManyThings from "../components/ManyThings.vue";
import TaoBaoMarket from "../components/TaoBaoMarket.vue";
/**
 * market组件
 * manytings组件
 */
export default {
  name: "Show",
  components: {
    TaoBaoMarket,
    ManyThings,
  },
};
</script>

<style>
.show-box{
display: flex;
flex-direction:row;
}
</style>