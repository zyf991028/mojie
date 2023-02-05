<script setup></script>

<template>
  <div class="middle">
    <img
      class="logo"
      src="https://www.baidu.com/img/PCtm_d9c8750bed0b3c7d089fa7d55720d6cf.png"
      alt="logo"
    />

    <div class="search-input">
      <input class="input" type="text" />
      <div class="search-button">百度一下</div>
    </div>
  </div>
</template>

<style scoped lang="less">
.middle {
  width: 100%;
  margin-top: 30px;
  display: flex;
  flex-direction: column;
  align-items: center;

  .logo {
    width: 270px;
    height: 129px;
    cursor: pointer;
  }

  .search-input {
    display: flex;
    margin-top: 20px;

    .input {
      width: 550px;
      height: 44px;
      border-radius: 10px 0 0 10px;
      border: 2px solid #c4c7ce;
      padding: 0px;
      border-right: 0px;
      outline: none;

      &:hover {
        border-color: #4e6ef2;
      }
    }

    .search-button {
      cursor: pointer;
      width: 130px;
      height: 48px;
      display: flex;
      align-items: center;
      justify-content: center;
      background-color: #4e6ef2;
      border-radius: 0 10px 10px 0;
      font-size: 17px;
      color: #fff;

      &:hover {
        background-color: fade(#4e6ef2, 80);
      }
    }
  }
}
</style>
