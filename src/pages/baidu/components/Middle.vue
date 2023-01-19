<script setup></script>

<template>
  <div class="footer">
    <div class="logo">
      <a href="https://www.baidu.com/"
        ><img
          src="https://www.baidu.com/img/PCtm_d9c8750bed0b3c7d089fa7d55720d6cf.png"
          width="300"
          height="140"
      /></a>
    </div>
    <div class="fond"><input type="text" /><button>百度一下</button></div>
  </div>
</template>

<style scoped lang="less">
.logo img {
  margin-top: 60px;
  margin-left: -330px;
}
input {
  width: 512px;
  height: 16px;
  padding: 12px 16px;
  font-size: 16px;
  margin: 0;
  border-radius: 10px 0 0 10px;
  border: 2px solid #c4c7ce;
  background: #fff;
  box-shadow: none;
  vertical-align: top;
  color: #222;
  overflow: hidden;
  box-sizing: content-box;
}
button {
  cursor: pointer;
  width: 120px;
  height: 44px;
  line-height: 25px;
  background-color: #4e6ef2;
  border-radius: 0 10px 10px 0;
  font-size: 17px;
  color: #fff;
}
</style>
