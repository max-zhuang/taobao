<template>
  <div class="Tmall-box">
    <div class="Tmall-tag-box">
      <a
        v-for="(p, index) of title1"
        :key="index"
        :href="p.url"
        :class="p.class"
        >{{ p.name }}</a
      >
    </div >
    |
    <div class="Tmall-tag-box">
      <a
        v-for="(p, index) of title2"
        :key="index"
        :href="p.url"
        :class="p.class"
        >{{ p.name }}</a
      >
    </div>
    |
    <div class="Tmall-tag-box">
      <a
        v-for="(p, index) of title3"
        :key="index"
        :href="p.url"
        :class="p.class"
        >{{ p.name }}</a
      >
    </div>
  </div>
</template>

<script>
export default {
  name: "Tmall",
  data() {
    return {
      title1: [
        { name: "天猫", url: "www.aaa.com", class: "R-box" },
        { name: "聚划算", url: "www.bbb.com", class: "R-box" },
        { name: "天猫超市", url: "www.ccc.com", class: "G-box" },
      ],
      title2: [
        { name: "司法拍卖", url: "www.ddd.com", class: "B-box" },
        { name: "飞猪旅行", url: "www.eee.com", class: "B-box" },
        { name: "天天特卖", url: "www.fff.com", class: "B-box" },
      ],
      title3: [
        { name: "造点新货", url: "www.ggg.com", class: "B-box" },
        { name: "苏宁易购", url: "www.hhh.com", class: "B-box" },
        { name: "淘宝心选", url: "www.iii.com", class: "B-box" },
        { name: "智能生活", url: "www.jjj.com", class: "B-box" },
      ],
    };
  },
};
</script>

<style>
.R-box {
  color: #ff0036;
  text-decoration: none;
  font-weight: 700;
  margin-right: 12px;
    margin-left: 12px;
}
.G-box {
  color: #33c900;
  text-decoration: none;
  font-weight: 700;
    margin-right: 12px;
    margin-left: 12px;
}
.Tmall-box {
  display: flex;
  margin: 10.72px 10.72px 10.72px 0;
  height: 23px;
  width: 900px;
  justify-content: space-around;
}

.Tmall-tag-box {
  display: flex;
  justify-content: space-around;
}
.B-box {
  color: #3c3c3c;
  text-decoration: none;
  font-weight: 400;
    margin-right: 12px;
    margin-left: 12px;
}
</style>