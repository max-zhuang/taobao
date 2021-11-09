<template>
  <div class="Hi">
    <div class="header">
      <img src="../assets/Hi-picture1.png" class="picture1" />
      <span style="font-size: 12px; margin-top: 4px; height: 17px"
        >Hi!你好</span
      >
    </div>
    <div class="link">
      <a
        v-for="(p, index) of UserInfor"
        :key="index"
        :href="p.url"
        :class="p.class"
        >{{ p.name }}</a
      >
    </div>

    <img
      src="../assets/Hi-picture2.png"
      style="height: 141px; width: 356px; margin: 0 14px 0 14px"
    />
  </div>
</template>

<script>
export default {
  data() {
    return {
      UserInfor: [
        { name: "登录", url: "www.qwe.com", class: "orange" },
        { name: "注册", url: "www.asd.com", class: "orange" },
        { name: "开店", url: "www.zxc.com", class: "orange" },
      ],
    };
  },
};
</script>

<style>
.Hi {
  display: flex;
  flex-direction: column;
  text-align: center;
}
.picture1 {
  display: flex;
  width: 50px;
  height: 50px;
  border-radius: 50%;
  margin: 20px auto 0;
}
.header {
  display: flex;
  flex-direction: column;
  width: 384px;
  height: 88px;
}
.link {
  display: flex;
  height: 42px;
  width: 372px;
  flex-direction: row;
  justify-content: space-around;
  margin: 11px 0 0 3px;
   align-items: center
}
.orange {
  text-decoration: none;
  color: #fff;
  background-color: #ff5000;
  height: 32px;
  width: 108px;
  border-radius: 4px;
  font-size: 16px;
  text-align: center;
}
</style>