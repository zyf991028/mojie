<script setup></script>

<template>
  <div class="header">
    <div class="left">
      <div><a href="https://news.baidu.com/">新闻</a></div>
      <div><a href="https://www.hao123.com/?src=from_pc/">hao123</a></div>
      <div><a href="https://map.baidu.com/@12529225,4152139,13z">地图</a></div>
      <div><a href="https://tieba.baidu.com/index.html">贴吧</a></div>
      <div><a href="https://haokan.baidu.com/?sfrom=baidu-top">视频</a></div>
      <div><a href="https://image.baidu.com/">图片</a></div>
      <div><a href="https://pan.baidu.com/?from=1026962h%2F">网盘</a></div>
      <div>
        <a href="https://www.baidu.com/more/">更多</a>
      </div>
    </div>
    <div class="right">
      <div>
        <button>
          <a
            href="https://passport.baidu.com/v2/?login&tpl=mn&u=http%3A%2F%2Fwww.baidu.com%2F&sms=5"
            >登录</a
          >
        </button>
      </div>
      <div>设置</div>
    </div>
  </div>
</template>

<style scoped lang="less">
.header {
  width: 100%;
  min-width: 1199px;
}
.left {
  div {
    margin-right: 24px;
    margin-top: 19px;
    float: left;
    font-size: 15px;
  }
}
.left div a {
  color: #000;
}
.left div a:hover {
  color: blue;
}

.right {
  div {
    margin-top: 19px;
    margin-right: 20px;
    float: right;
    font-size: 15px;
  }
}
.right div:hover {
  color: blue;
}
button {
  width: 60px;
  height: 24px;
  font-size: 13px;
  margin-top: 0px;
  margin-right: -35px;
}
.right div button {
  background-color: #4e71f2;
}
.right div a {
  color: white;
}
.caidan {
  display: none;
  position: absolute;
  top: 29px;
  right: -12px;
  width: 228px;
  height: 298px;
  background: #fff;
  box-shadow: 0 2px 10px 0 rgb(0 0 0 /15%);
  border-radius: 12px;
}
</style>
