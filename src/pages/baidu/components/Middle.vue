<script setup>
const srca = [
  {
    link: "https://www.baidu.com",
  },
];
const imgs = (src) => {
  window.open(src, "__BLANK");
};
</script>

<template>
  <div class="middle">
    <div class="logo" v-for="srcs in srca" @click="imgs(srcs.link)">
      {{ srcs.title }}
      <img
        src="https://www.baidu.com/img/PCtm_d9c8750bed0b3c7d089fa7d55720d6cf.png"
        alt=""
      />
    </div>
    <div class="inputs"><button>百度一下</button></div>
  </div>
</template>

<style scoped lang="less">
.middle {
  width: 100%;
  height: 250px;
  position: absolute;
  .logo {
    width: 270px;
    height: 129px;
    display: flex;
    margin: auto;
    cursor: pointer;
  }
  .inputs {
    position: relative;
    left: 25%;
    top: 10%;
    width: 443px;
    height: 16px;
    padding: 12px 16px;
    border-radius: 10px 0 0 10px;
    border: 2px solid #c4c7ce;
    display: flex;
    text-align: center;
  }
  .inputs button {
    position: relative;
    left: 104%;
    top: -88%;
    cursor: pointer;
    width: 120px;
    height: 44px;
    line-height: 44px;
    background-color: #4e6ef2;
    border-radius: 0 10px 10px 0;
    border: 2px solid #c4c7ce;
    font-size: 17px;
    color: #fff;
  }
}
</style>
