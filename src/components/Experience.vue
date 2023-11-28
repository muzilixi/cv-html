<template>
  <table class="home-experience">
    <tr>
      <th width="16%"></th>
      <th width="39%" class="experience-border-top"></th>
      <th width="39%" class="experience-border-top"></th>
    </tr>
    <tr>
      <td>2023.4至今</td>
      <td>软通动力信息技术(外派宁德时代)</td>
      <td></td>
    </tr>
    <tr>
      <td>2022.7-2023.2</td>
      <td>锐明技术有限公司</td>
      <td></td>
    </tr>
    <tr>
      <td>2018.8-2022.7</td>
      <td>德勤</td>
      <td></td>
    </tr>
    <tr>
      <td>2017.6-2018.8</td>
      <td>阳光信用保证保险股份有限公司</td>
      <td></td>
    </tr>
    <tr>
      <td>2013.9-2017.6</td>
      <td class="experience-border-bottom">长江师范学院</td>
      <td class="experience-border-bottom">英语四级 创新创业团队负责人</td>
    </tr>
  </table>
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
.home-experience {
  margin-top: var(--main-margin);
  width: 100%;
  font-weight: 600;
  color: var(--main-color);
  tr {
    td {
      line-height: 26px;
    }
  }

  .experience-border-top {
    border-top: var(--main-border);
    padding-top: var(--main-padding);
  }

  .experience-border-bottom {
    border-bottom: var(--main-border);
    padding-bottom: var(--main-padding);
  }
}
</style>
