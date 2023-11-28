<template>
  <div class="home-header">
    <span class="header-name">李 熺</span>
    <span class="header-sub">求职意向:</span>
    <span class="header-sub-text">IT开发工程师-Web前端</span>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
};
</script>

<style scoped lang="less">
.home-header {
  margin-top: var(--sub-margin);
  color: var(--main-color);
  vertical-align: bottom;
  .header-name {
    font-size: 40px;
    font-weight: 600;
    display: inline-block;
    width: 140px;
    border-bottom: var(--main-border);
  }
  .header-sub {
    font-size: 16px;
    font-weight: 500;
    padding-left: 20px;
    position: relative;
    top: 9px;
  }
  .header-sub-text {
    padding-left: 20px;
    font-size: 16px;
    font-weight: 700;
    position: relative;
    top: 9px;
  }
}
</style>
