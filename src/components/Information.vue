<template>
  <div class="information">
    <Hi/>
    <Notice/>
    </div>
</template>

<script>
import Hi from '../components/Hi.vue'
import Notice from '../components/Notice.vue'
export default {
  name:"Information",
  components:{
   Hi,Notice
  }
}
</script>

<style>
.information{
  display: flex;
  flex-direction: column;
  width: 384px;
  height: 508px;
  border-radius: 12px;
  margin-right: 18px;
  margin-top: 10px;
  margin-left: 33px;
  background-color: #f3f3f3;
  text-align:center

}
</style>