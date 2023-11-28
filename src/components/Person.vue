<template>
  <div class="home-person">
    <img class="person-img" src="../assets/blue02.jpg" alt="" />
    <table class="home-person-content">
      <tr>
        <th width="7%"></th>
        <th width="2%"></th>
        <th width="41%"></th>
        <th width="12%"></th>
        <th width="2%"></th>
        <th width="38%"></th>
      </tr>
      <tr>
        <td class="person-label">籍贯</td>
        <td class="person-label-icon">:</td>
        <td class="person-text">重庆</td>
        <td class="person-label">工作年限</td>
        <td class="person-label-icon">:</td>
        <td class="person-text">7年</td>
      </tr>
      <tr>
        <td class="person-label">年龄</td>
        <td class="person-label-icon">:</td>
        <td class="person-text">30</td>
        <td class="person-label">学历</td>
        <td class="person-label-icon">:</td>
        <td class="person-text">本科</td>
      </tr>
      <tr>
        <td class="person-label">学校</td>
        <td class="person-label-icon">:</td>
        <td class="person-text">长江师范学院</td>
        <td class="person-label">专业</td>
        <td class="person-label-icon">:</td>
        <td class="person-text">计算机科学与技术</td>
      </tr>
      <tr>
        <td class="person-label">邮箱</td>
        <td class="person-label-icon">:</td>
        <td class="person-text">269 081 6541@qq.com</td>
        <td class="person-label">电话</td>
        <td class="person-label-icon">:</td>
        <td class="person-text">182 2371 0570</td>
      </tr>
    </table>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    data: [{}],
  },
};
</script>

<style scoped lang="less">
.home-person {
  position: relative;
  .person-img {
    position: absolute;
    right: 0px;
    width: 116px;
    top: -50px;
  }
  .home-person-content {
    width: 70%;
    margin-top: var(--sub-margin);

    tr {
      td {
        line-height: 28px;
      }
    }

    .person-label {
      text-align: justify;
      text-align-last: justify;
    }

    .person-label-icon {
      text-align: center;
    }

    .person-text {
      font-weight: 600;
    }
  }
}
</style>
