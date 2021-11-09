<template>
  <div class="bigimage-box">
    <FirstImg />
    <SecondImg />
  </div>
</template>

<script>
import FirstImg from "../components/FirstImg.vue";
import SecondImg from "../components/SecondImg.vue";
export default {
  name: "BigImage",
  components: {
    FirstImg,
    SecondImg,
  },
};
</script>

<style>
.bigimage-box {
  display: flex;
  flex-direction: column;
}
</style>