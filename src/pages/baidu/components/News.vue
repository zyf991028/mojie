<script setup>
const news = [
  {
    link: "#",
    title: "1春节临近 各种多措并举保供稳价",
  },
  {
    link: "#",
    title: "2乙类乙管后 重症救治等情况如何",
  },
  {
    link: "#",
    title: "3尼泊尔一载72人客机坠毁 现场曝光",
  },
  {
    link: "#",
    title: "4多人因假冒王思聪行骗被判刑",
  },
  {
    link: "#",
    title: "5如果今天无罪,明天就出车",
  },
  {
    link: "#",
    title: "6尼泊尔坠机现场已找到30具遗体",
  },
];
const navigate = (src) => {
  window.open(src, "__BLANK");
};
</script>

<template>
  <div class="news-container">
    <div class="action">
      <div class="left"><b>百度热搜</b></div>
      <div class="right">换一换</div>
    </div>
    <div class="news-content">
      <div
        class="news-link"
        v-for="newItem in news"
        @click="navigate(newItem.link)"
      >
        {{ newItem.title }}>
      </div>
    </div>
  </div>
</template>

<style scoped lang="less">
.news-container {
  width: 100%;
  margin-top: 40px;
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  flex-direction: column;
  align-items: center;
  cursor: pointer;

  .action {
    width: 500px;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;

    .left:hover {
      color: #315efb;
    }

    .right {
      color: #626675;
    }

    .right:hover {
      color: #315efb;
    }
  }

  .news-content {
    width: 500px;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;

    .news-link {
      width: 220px;
      height: 40px;
      line-height: 40px;
      overflow: hidden;
      text-overflow: ellipsis;
      white-space: nowrap;

      &:hover {
        color: #315efb;
      }
    }
  }
}
</style>
