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
      <div class="menu-item">
        <a href="">设置</a>
        <div class="content">
          <a href="javascript:;">搜索设置</a>
          <a href="https://www.baidu.com/gaoji/advanced.html">高级搜索</a>
          <a href="javascript:;">关闭预测</a>
          <a
            href="https://passport.baidu.com/v2/?login&tpl=pc&extrajson=%7B%22l%22%3A%22%22%2C%22s%22%3A%22%22%2C%22src%22%3A%22se_070003%22%7D&u=https%3A%2F%2Fwww.baidu.com%2Fduty%2Fprivacysettings.html"
            >隐藏设置</a
          >
          <a href="javascript:;">关闭热搜</a>
        </div>
      </div>

      <div class="login-btn" @click="navigate(loginUrl)">登录</div>
    </div>
  </div>
</template>

<style scoped lang="less">
.header {
  width: 100%;
  margin-top: 20px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0px 24px;
  box-sizing: border-box;

  .menu-item {
    display: inline-block;

    &:not(:last-child) {
      margin-right: 24px;
    }

    a {
      color: #333;
      font-size: 12px;
      cursor: pointer;
    }

    a:hover {
      color: #4e6ef2;
    }

    .content {
      display: none;
      position: absolute;
      right: 70px;
      background-color: #fff;
      box-shadow: 0 0 10px #d7d9e0;
      color: #333;
      width: 84px;
      text-align: center;
      border-radius: 12px;
    }

    .content a {
      display: block;
      text-decoration: none;
    }

    &:hover {
      top: 6px;
    }

    &:hover .content {
      display: block;
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
