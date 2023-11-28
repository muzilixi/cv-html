<template>
  <div class="home-skill">
    <ul>
      <li>熟练掌握： React及其底层实现原理 ahooks ant-design</li>
      <li>熟练掌握： Vue2 Vue3及其底层实现原理 element-ui</li>
      <li>熟练掌握： amap leaflet echarts webpack 移动端适配</li>
      <li>熟练掌握： typescript es6 css3 html，</li>
      <li class="title"><span>个人优势：</span></li>
      <li>
        <label for="">熟练掌握相关知识，代码规范</label>
        <label for="">优化项目，提高项目开发效率和可维护性</label>
        <label for=""
          >微前端架构、参与项目选型、开发公共组件优化框架、实现自己的ui库</label
        >
      </li>
    </ul>
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
.home-skill {
  margin-top: var(--main-margin);
  border-top: var(--main-border);
  border-bottom: var(--main-border);
  padding: var(--main-padding) 0;
  ul {
    li {
      color: var(--main-color);
      font-weight: 600;
      line-height: 36px;
      &.title {
        padding-top: 12px;
        padding-left: 8px;
        span {
          display: inline-block;
          transform: scale(1.2);
        }
      }
      label {
        display: block;
        padding-left: 48px;
      }
    }
  }
}
</style>
