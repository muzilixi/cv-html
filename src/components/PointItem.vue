<template>
  <div class="point-item-com">
    <h3 @click="handleClick">{{ title }}</h3>
    <div class="point-img"
         v-show="show">
      <img v-for="item in images"
           :src="item"
           :key="item"
           alt=" ">
    </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    title: {
      type: String,
      default: '项目选型后前期准备'
    },
    images: {
      type: [Array],
      default: () => ['../assets/图片1.png']
    }
  },
  data() {
    return {
      show: false,
    }
  },
  methods: {
    handleClick() { this.show = !this.show }
  }
}
</script>

<style scoped lang="less">
.point-item-com {
  h3 {
    color: var(--main-color);
    line-height: 32px;
    cursor: pointer;
  }
  .point-img {
    img {
      width: 100%;
    }
  }
}
</style>
