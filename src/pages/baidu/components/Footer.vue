<script setup>
const under = [
  {
    link: "https://home.baidu.com/",
    title: "关于百度",
  },
  {
    link: "https://ir.baidu.com/",
    title: "About&nbsp;Baidu",
  },
  {
    link: "https://www.baidu.com/duty/",
    title: "使用百度前必读",
  },
  {
    link: "https://help.baidu.com/",
    title: "帮助中心",
  },
  {
    link: "https://e.baidu.com/?refer=1271",
    title: "企业推广",
  },
  {
    link: "https://www.beian.gov.cn/portal/registerSystemInfo?recordcode=11000002000001",
    title: "京公网安备11000002000001号",
  },
  {
    link: "https://beian.miit.gov.cn/#/Integrated/index",
    title: "京ICP证030173号",
  },
  {
    link: "https://www.baidu.com/licence/",
    title: "信息网络传播视听节目许可证0110516",
  },
];
const opens = (src) => {
  window.open(src, "_BLANK");
};
</script>

<template>
  <div class="footer">
    <div class="footers" v-for="up in under" @click="opens(up.link)">
      {{ up.title }}
    </div>
  </div>
</template>

<style scoped lang="less">
.footer {
  width: 100%;
  height: 30px;
  position: fixed;
  bottom: 0;
  display: flex;
  cursor: pointer;
  text-align: center;
  .footers {
    color: #9195a3;
    float: left;
    font-size: 12px;
    margin-left: 50px;
  }
  .footers:hover {
    color: #000;
  }
}
</style>
