<template>
  <div class="home-point">
    <PointItem
      v-for="item in data"
      :key="item.title"
      :title="item.title"
      :images="item.images"
    />
  </div>
</template>

<script>
import PointItem from "./PointItem.vue";
export default {
  name: "HelloWorld",
  components: { PointItem },
  data() {
    return {
      data: [
        {
          title: "项目选型后前期准备",
          images: [require("../assets/图片1.png")],
        },
        {
          title: "组件封装",
          images: [
            require("../assets/图片2.png"),
            require("../assets/图片3.png"),
            require("../assets/图片4.png"),
          ],
        },
        {
          title: "实现自己的 ui 库",
          images: [require("../assets/图片5.png")],
        },
        {
          title: "公共方法",
          images: [require("../assets/图片6.png")],
        },
        {
          title: "代码优化",
          images: [require("../assets/图片7.png")],
        },
      ],
    };
  },
};
</script>

<style scoped lang="less">
.home-point {
  margin-top: var(--main-margin);
  border-top: var(--main-border);
  border-bottom: var(--main-border);
  padding: var(--main-padding) 0;
}
</style>
