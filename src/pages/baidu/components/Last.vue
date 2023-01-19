<script setup></script>

<template>
  <div class="last">
    <div class="shang">
      <div><b>百度热搜</b>&nbsp;<span>换一换</span></div>
    </div>
    <div class="left">
      <div>1&nbsp;&nbsp;&nbsp;&nbsp;春节临近 各种多措并举保供稳价</div>
      <div>2&nbsp;&nbsp;&nbsp;&nbsp;乙类乙管后 重症救治等情况如何</div>
      <div>3&nbsp;&nbsp;&nbsp;&nbsp;尼泊尔一载72人客机坠毁 现场曝光</div>
    </div>
    <div class="right">
      <div>4&nbsp;&nbsp;&nbsp;&nbsp;多人因假冒王思聪行骗被判刑</div>
      <div>5&nbsp;&nbsp;&nbsp;&nbsp;如果今天无罪,明天就出车</div>
      <div>6&nbsp;&nbsp;&nbsp;&nbsp;尼泊尔坠机现场已找到30具遗体</div>
    </div>
  </div>
  <div class="clear"></div>
</template>

<style scoped lang="less">
.last .shang div {
  margin-top: 40px;
  margin-left: 10px;
}
.last .shang div span {
  margin-left: 600px;
}
.last .shang div b:hover {
  color: blue;
}
.last .shang div span:hover {
  color: blue;
}
.last .left div:hover {
  color: blue;
}
.last .left {
  float: left;
  margin-left: 200px;
}
.last .right {
  float: right;
  margin-right: 200px;
}
.last .right div:hover {
  color: blue;
}
.last div {
  margin-top: 10px;
}
.clear {
  clear: both;
}
</style>
