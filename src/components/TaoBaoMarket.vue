<template>
  <div class="Market-box">
    <h1 class="h-box">主题市场</h1>
    <div class="tags-box">
      <a
        el-icon-goods
        v-for="(p, index) of MarketTags"
        :key="index"
        :href="p.url"
        class="market-link"
        >{{ p.name }} /</a
      >
    </div>
  </div>
</template>

<script>
export default {
  name: "TaobaoMarket",
  data() {
    return {
      MarketTags: [
        { name: "女装", url: "www.111.com" },
        { name: "内衣", url: "www.222.com" },
        { name: "家居", url: "www.333.com" },
        { name: "女鞋", url: "www.444.com" },
        { name: "男鞋", url: "www.555.com" },
        { name: "箱包", url: "www.666.com" },
        { name: "母婴", url: "www.777.com" },
        { name: "童装", url: "www.888.com" },
        { name: "玩具", url: "www.999.com" },
        { name: "女装", url: "www.111.com" },
        { name: "内衣", url: "www.222.com" },
        { name: "家居", url: "www.333.com" },
        { name: "女鞋", url: "www.444.com" },
        { name: "男鞋", url: "www.555.com" },
        { name: "箱包", url: "www.666.com" },
        { name: "母婴", url: "www.777.com" },
        { name: "童装", url: "www.888.com" },
        { name: "玩具", url: "www.999.com" },
        { name: "女装", url: "www.111.com" },
        { name: "内衣", url: "www.222.com" },
        { name: "家居", url: "www.333.com" },
        { name: "女鞋", url: "www.444.com" },
        { name: "男鞋", url: "www.555.com" },
        { name: "箱包", url: "www.666.com" },
        { name: "母婴", url: "www.777.com" },
        { name: "童装", url: "www.888.com" },
        { name: "玩具", url: "www.999.com" },
        { name: "女装", url: "www.111.com" },
        { name: "内衣", url: "www.222.com" },
        { name: "家居", url: "www.333.com" },
        { name: "女鞋", url: "www.444.com" },
        { name: "男鞋", url: "www.555.com" },
        { name: "箱包", url: "www.666.com" },
        { name: "母婴", url: "www.777.com" },
        { name: "童装", url: "www.888.com" },
        { name: "玩具", url: "www.999.com" },
        { name: "女装", url: "www.111.com" },
        { name: "内衣", url: "www.222.com" },
        { name: "家居", url: "www.333.com" },
        { name: "女鞋", url: "www.444.com" },
        { name: "男鞋", url: "www.555.com" },
        { name: "箱包", url: "www.666.com" },
        { name: "母婴", url: "www.777.com" },
        { name: "童装", url: "www.888.com" },
        { name: "玩具", url: "www.999.com" },
        { name: "女装", url: "www.111.com" },
        { name: "内衣", url: "www.222.com" },
        { name: "家居", url: "www.333.com" },
        { name: "女鞋", url: "www.444.com" },
        { name: "男鞋", url: "www.555.com" },
        { name: "箱包", url: "www.666.com" },
      ],
    };
  },
};
</script>

<style>
.h-box {
  color: rgb(255, 80, 0);
  font-size: 16px;
  width: 212px;
  text-align: center;
}
.tags-box {
  display: flex;
  flex-wrap: wrap;
  flex-direction: row;
  width: 185px;
  justify-content: space-between;
  margin: 10px;
}
.Market-box {
  width: 212px;
  height: 549px;
}
.market-link {
  font-size: 14px;
  font-weight: 400;
  width: 33.3%;
  color: #666;
  text-decoration: none;
  margin-bottom: 10px;
}
</style>