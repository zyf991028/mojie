<script setup>
const menuList = [
  {
    link: "https://news.baidu.com/",
    title: "新闻",
  },
  {
    link: "https://www.hao123.com/?src=from_pc/",
    title: "hao123",
  },
  {
    link: "https://map.baidu.com/@12529225,4152139,13z",
    title: "贴吧",
  },
  {
    link: "https://haokan.baidu.com/?sfrom=baidu-top",
    title: "视频",
  },
  {
    link: "https://image.baidu.com/",
    title: "图片",
  },
  {
    link: "https://pan.baidu.com/?from=1026962h%2F",
    title: "网盘",
  },
  {
    link: "https://www.baidu.com/more/",
    title: "更多",
  },
];

const loginUrl =
  "https://passport.baidu.com/v2/?login&tpl=mn&u=http%3A%2F%2Fwww.baidu.com%2F&sms=5";

const navigate = (src) => {
  window.open(src, "__BLANK");
};
</script>

<template>
  <div class="header">
    <div class="menu-container">
      <div
        class="menu-item"
        v-for="menuItem in menuList"
        @click="navigate(menuItem.link)"
      >
        {{ menuItem.title }}
      </div>
    </div>

    <div class="action-container">
      <div class="menu-item">设置</div>

      <div class="login-btn" @click="navigate(loginUrl)">登录</div>
    </div>
  </div>
</template>

<style scoped lang="less">
.header {
  width: 100%;
  height: 60px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0px 24px;
  box-sizing: border-box;

  .menu-item {
    font-size: 12px;
    color: #000;
    cursor: pointer;

    &:not(:last-child) {
      margin-right: 24px;
    }

    &:hover {
      color: blue;
    }
  }

  .menu-container {
    display: flex;
  }

  .action-container {
    display: flex;
    align-items: center;

    .login-btn {
      font-size: 12px;
      border-radius: 4px;
      background-color: #4e6ef2;
      display: flex;
      justify-content: center;
      align-items: center;
      color: #fff;
      padding: 4px 12px;
      cursor: pointer;
    }
  }
}
</style>
