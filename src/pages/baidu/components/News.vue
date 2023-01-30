<script setup>
const neww = [
  { link: "#", title: "1春节临近 各种多措并举保供稳价" },
  { link: "#", title: "2乙类乙管后 重症救治等情况如何" },
  { link: "#", title: "3尼泊尔一载72人客机坠毁 现场曝光" },
  { link: "#", title: "4多人因假冒王思聪行骗被判刑" },
  { link: "#", title: "5如果今天无罪,明天就出车" },
  { link: "#", title: "6尼泊尔坠机现场已找到30具遗体" },
];
const newa = (src) => {
  window.open(src, "__BLANK");
};
</script>

<template>
  <div class="news">
    <div class="shang" v-for="shangs in neww" @click="newa(shangs.link)">
      {{ shangs.title }}
    </div>
    <div class="xia" v-for="xias in neww" @click="newa(xias.link)">
      {{ xias.title }}
    </div>
  </div>
</template>

<style scoped lang="less">
.news {
  width: 100%;
  height: 150px;
  margin-top: 260px;
  cursor: pointer;
  text-align: center;
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
}
</style>
