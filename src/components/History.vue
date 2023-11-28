<template>
  <div class="home-history">
    <div class="history-item" v-for="item in data" :key="item.project">
      <h3>
        <span class="history-project">{{ item.project }}</span>
        <span class="history-company">{{ item.company }}</span>
        <span class="history-job">{{ item.job }}</span>
      </h3>
      <div class="history-desc">
        <span class="history-label">描述：</span>{{ item.desc }}
      </div>
      <div class="history-desc">
        <span class="history-label">技术栈：</span>{{ item.skill }}
      </div>
      <div class="history-label content">工作内容：</div>
      <ul
        v-for="(contentItem, contentIndex) in item.content"
        :key="contentIndex"
      >
        <li>{{ contentIndex + 1 }}. {{ contentItem }}</li>
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
          project: "星河一站式",
          company: "宁德时代新能源",
          job: "前端开发",
          desc: "星河一站式开发包含星河后台管理系统、天眼系统、星河一站式前台",
          skill: "umi.React, echarts, ahooks, antd",
          content: [
            "开发通用组件（后台系统表单组件、文件上传组件、富文本组件等，前台滚动组件、空状态组件等）",
            "前台后台工作台配置功能，实现各业务卡片自定排版",
            "新闻模块,后台系统配置新闻通过富文本方式维护新闻模块",
            "DEDA模块，后台系统配置DEDA内容，前台展示及页面相关动画交互",
            "卡片，星河一站式卡片模块达人币&快捷卡片等",
            "天眼系统，后台提交系统及管理端系统",
          ],
        },
        {
          project: "业务中台",
          company: "锐明技术有限公司",
          job: "前端开发",
          desc: "管控平台，平台司机、车辆、租户等信息维护",
          skill: "React函数组件, echarts, leaflet, ahooks, antd",
          content: [
            "开发公用表单，表格等组件",
            "通过车辆gps数据绘制车辆行程等信息",
          ],
        },
        {
          project: "基于阿里云中台的物流系统",
          company: "中兴",
          job: "前端负责人",
          desc: "基于阿里云的物流系统继承各个外部系统基础数据开发网站并实现国际化",
          skill: "Vue-cli, Vue, Elemet",
          content: [
            "使用 Vue-cli 脚手架搭建项目完成路由，store，公共方法等框架模块",
            "在 element 组件基础上封装更适与系统的表单表格等组件",
            "安排前端同时负责不同模块的页面完成",
            "与后端人员对接实现页面的权限接入及其他模块接口对接",
          ],
        },
        {
          project: "鹏鼎数据专案",
          company: "鹏鼎鹏鼎",
          job: "前端负责人",
          desc: "一套报表系统，集成 echarts 中折线图、柱状图、水晶球、地图等多种图表",
          skill: "Vue-cli, Vue, Elemet, echarts, axios",
          content: [
            "基于 vue-element-admin 搭建前端框架",
            "封装通用基础组件",
            "带领前端人员一起完成页面布局展示",
            "使用 axios 对接后端服务",
            "将项目部署到远程服务器并发布",
          ],
        },
        {
          project: "德勤 tax bps",
          company: "德勤",
          job: "前端开发",
          desc: "报销统计系统负责借款、还款、费用报销、对公付账等模块申请、审批、财务审批、出纳付款入账开发",
          skill: "react-cli, react, Redux-thunk, immutable, react-loadable",
          content: [
            "使用 react-cli 搭建前端框架",
            "完成通用组件的封装",
            "使用 Redux-thunk 中间件书写 redux 管理统一数据",
            "使用 react-loadable 组件一部加载页面",
          ],
        },
        {
          project: "宝马 UCOR",
          company: "宝马",
          job: "前端开发",
          desc: "宝马的一套及权限、生产、物料、报表系统",
          skill: "vue-cli, vue, vue-router, vuex, axios, echarts, spreadJs",
          content: [
            "使用 echarts 多种图标完成报表系统首页",
            "使用 spreadJs 模拟 excel 完成页面及页面中的表格模块",
            "封装并且基础组件使得多个页面开发效率提高并且样式统一",
          ],
        },
      ],
    };
  },
};
</script>

<style scoped lang="less">
.home-history {
  margin-top: var(--main-margin);
  border-top: var(--main-border);
  border-bottom: var(--main-border);
  .history-item {
    border-bottom: var(--sub-border);
    padding-bottom: 14px;
    &:last-child {
      border-bottom: none;
    }
    h3 {
      color: var(--main-color);
      line-height: 32px;
      .history-project {
        display: inline-block;
        width: 40%;
      }
      .history-company {
        display: inline-block;
        width: 20%;
      }
      .history-job {
        display: inline-block;
        width: 40%;
      }
    }
    .history-desc {
      font-weight: 600;
      line-height: 32px;
    }
    .history-label {
      font-weight: 700;
      &.content {
        padding: 8px 0 8px;
      }
    }
    ul {
      li {
        line-height: 26px;
      }
    }
  }
}
</style>
