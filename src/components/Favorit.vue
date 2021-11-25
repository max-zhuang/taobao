<template>
  <div class="fav">
  <a v-for="(p,index) of products" :key="index" class="fav-a">
    <img :src="p.imgUrl" class="fav-img"/>
    <span class="fav-des">{{p.des}}</span>
    <span class="fav-price">{{p.price}}</span>
    </a>  
  </div>
</template>

<script>
import axios from 'axios'
export default {
data() {
  return {
    products:[]
  }
},
mounted() {

  axios.get('http://zhuangmaoxuexi.5gzvip.91tunnel.com/list_products')
  .then ( (response)=> {
    this.products=response.data;
  })


},
}
</script>

<style>
.fav-img{
  display: flex;
  flex-direction: column;
  width: 215px;
  height: 215px;
}
.fav{
  display: flex;
  flex-direction: row;
  width: 1190px;
  flex-wrap: wrap
}
.fav-a{
  border-radius: 12px;
    float: left;
    padding: 7px 7px 0 7px;
    margin: 0 0 2px 7px;
    color: #6c6c6c;
    width: 215px;
    height: 319px;
    position: relative;
}
.fav-des{
  display: flex;
  margin-top: 9px;
  line-height: 22px;
  height: 44px;
  font-size: 16px;
  color: #111111;
  font-weight: normal;
  transition: color 0.3s;
  overflow: hidden;
}
.fav-price{
  float: left;
    color: #F40;
    font-size: 20px;
    height: 22px;
    line-height: 22px;
}
</style>