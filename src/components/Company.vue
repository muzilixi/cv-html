<template>
  <div class="home-company">
    <div class="company-item" v-for="item in data" :key="item.title">
      <h3>{{ item.title }}</h3>
      <div class="company-skill">技术： {{ item.skill }}</div>
      <ul>
        <li v-for="(contentItem, index) in item.content" :key="contentItem">
          {{ index + 1 }}. {{ contentItem }}
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {},
  data() {
    return {
      data: [
        {
          title: "锐明技术有限公司",
          skill: "react Antd ahooks leaflet",
          content: [
            "设计公共开发组件 出相关设计文档 开发公用的组件",
            "管理项目资源 参与代码评审 优化项目框架等",
            "项目部署",
          ],
        },
        {
          title: "德勤",
          skill: "Vue React Element Vant Antd",
          content: [
            "基于 vue-ci、 react-cli 搭建前端框架，完成基本路由、Store，数据请求等配置",
            "在框架中完成公共 css、公共通用方法，过滤器等",
            "完成通用组件的封装",
            "完成基本页面的开发，前后端接口联调",
            "远程服务器自动化配置发布前端项目",
            "负责前端开发任务拆解与分配，前端开发进度管理以及问题解决",
            "辅导实习生及前端人员开发所分配模块",
          ],
        },
        {
          title: "阳光信用保证保险",
          skill: "Vue H5 Css3 Jquery",
          content: [
            "CDN方式使用 Vue 开发公司官网",
            "使用 Css3 动画实现官网首页各模块动画",
            "与后端数据联调",
            "使用 flexible 移动端自适应方案完成官网微信服务号开发",
          ],
        },
      ],
    };
  },
};
</script>

<style scoped lang="less">
.home-company {
  margin-top: var(--main-margin);
  border-top: var(--main-border);
  border-bottom: var(--main-border);
  .company-item {
    padding-top: var(--main-padding);
    border-bottom: var(--sub-border);
    padding-bottom: 14px;
    &:last-child {
      border-bottom: none;
    }
    h3 {
      color: var(--main-color);
      line-height: 32px;
    }
    .company-skill {
      font-weight: 600;
      line-height: 32px;
    }
    ul {
      li {
        line-height: 26px;
      }
    }
  }
}
</style>
