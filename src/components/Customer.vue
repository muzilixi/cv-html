<template>
  <div class="home-customer">
    <span class="sub-tip">主要客户：</span>
    <span class="company-item" v-for="item in data" :key="item">{{
      item
    }}</span>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
  data() {
    return {
      data: [
        "宁德时代新能源科技股份有限公司",
        "华为",
        "阿里",
        "中兴",
        "舍弗勒",
        "宝马",
      ],
    };
  },
};
</script>

<style scoped lang="less">
.home-customer {
  margin-top: var(--main-margin);
  font-weight: 600;
  color: var(--main-color);
  border-top: var(--main-border);
  border-bottom: var(--main-border);
  line-height: 36px;
  display: flex;
  gap: 0 16px;
  .sub-tip {
    font-weight: normal;
  }
}
</style>
