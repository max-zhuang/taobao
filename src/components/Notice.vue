<template>
  <div>
    <div class="notice-top">
      <span  class="notice-title">公告</span>
      <span class="notice-desc">新鲜事都在这里~</span>
    </div>
    <div v-for="(p,index) of hottag" :key="index" class="notice-content">
     <span class="notice-tip">热点</span><a :href="p.url" class="notice-content-a">{{p.title}}</a>
    </div>
  
  <div  class="rec">
    <div ><a href="https://shoucang.taobao.com/item_collect.htm" class="mytao-content"><span ></span><p>收藏的宝贝</p></a></div>
    <div ><a href="https://favorite.taobao.com/list_bought_shops_n.htm" class="mytao-content"><span ></span><p>买过的店铺</p></a></div>
    <div ><a href="https://shoucang.taobao.com/shop_collect_list_n.htm" class="mytao-content"><span ></span><p >收藏的店铺</p></a></div>
    <div ><a href="https://www.taobao.com/markets/footmark/tbfoot" class="mytao-content"><span></span><p>我的足迹</p></a></div>
</div>
  </div>
  
</template>

<script>
export default {
  data(){
    return{
      hottag:[
        {title:"【规则】2021年淘宝11.11招商规则",url:"www.123.com"},
        {title:"关于推进“清朗”账号乱象专项整治的通知",url:"www.456.com"},
        {title:"《淘宝平台违禁信息管理规则》规则变更通知",url:"www.789.com"},
      ]
    }
  }

}
</script>

<style>
.notice-top{
    display: flex;
    margin: 17px 0 14px 14px;
    height: 16px;
    line-height: 16px;
    justify-content: flex-start
}
.notice-title{ 
    height: 16px;
    font-size: 12px;
    line-height: 16px;
    font-weight: 700;
}
.notice-desc{
    margin-left:6px;
    height: 16px;
    font-size: 12px;
    line-height: 16px;
}
.notice-content{
    display: flex;
    margin-bottom: 8px;
    line-height: 18px;
    height: 18px;
    position: relative;
    overflow: hidden;
    flex-direction: row;
    margin-left: 14px;
}
.notice-content-a{
  display: flex;
  font-size: 12px;
    color: #666;
    margin-left: 8px;
    float: left;
    width: 295px;
    text-overflow: ellipsis;
    white-space: nowrap;
    overflow: hidden;
    margin-left:8px ;
    justify-content: flex-start;
    text-decoration: none;
}
.notice-tip{
  height: 18px;
    width: 32px;
    line-height: 18px;
    border-radius: 2px;
    background-color: rgba(255,174,174,.2);
    opacity: .8;
    text-align: center;
    font-size: 12px;
    color: #FF5000;
    font-weight: 700;
    float: left;
    text-emphasis: none;

}
.mytao{
  float: left;
  margin-right: 43px;
}
.rec{
  display: flex;
  flex-direction: row;
  margin-left: 14px;
  justify-content: space-around;
  
}
.mytao-conect{
  display: flex;
text-emphasis: none;
color: #f3f3f3;
}
</style>