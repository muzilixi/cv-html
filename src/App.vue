<template>
  <div class="page-home">
    <div class="page-home-content">
      <Header />
      <Person />
      <Experience />
      <Skill />
      <Customer />
      <Company />
      <History />
      <Point />
    </div>
    <div class="page-home-icon"></div>
    <div class="page-home-icon-round"></div>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Person from "./components/Person.vue";
import Experience from "./components/Experience.vue";
import Skill from "./components/Skill.vue";
import Customer from "./components/Customer.vue";
import Company from "./components/Company.vue";
import History from "./components/History.vue";
import Point from "./components/Point.vue";

export default {
  name: "App",
  components: {
    Header,
    Person,
    Experience,
    Skill,
    Customer,
    Company,
    History,
    Point,
  },
};
</script>

<style lang="less">
:root {
  --main-color: #271f4d;
  --main-border: 4px solid #2c3f71;
  --sub-border: 1px #2c3f71 dashed;
  --main-box-shadow: 0px 0px 4px 4px rgba(0, 0, 0, 0.1);
  --main-margin: 34px;
  --sub-margin: 8px;
  --main-padding: 8px;
}
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-size: 16px;
}
table {
  border-collapse: collapse;
}
ul,
li {
  list-style: none;
}
.page-home {
  width: 1000px;
  margin: 0 auto;
  box-shadow: var(--main-box-shadow);
  padding: 26px;
  overflow: hidden;
  position: relative;
  min-height: 800px;
  border: 1px solid rgba(0, 0, 0, 0.1);
  .page-home-icon {
    position: absolute;
    right: -80px;
    top: -80px;
    width: 160px;
    height: 160px;
    background-color: var(--main-color);
    transform: rotate(45deg);
  }
  .page-home-icon-round {
    position: absolute;
    right: -80px;
    top: 70px;
    width: 300px;
    height: 20px;
    background-color: var(--main-color);
    transform: rotate(45deg);
  }
  .page-home-content {
    box-shadow: var(--main-box-shadow);
    padding: 30px;
    overflow: hidden;
    min-height: 800px;
    border: 1px solid rgba(0, 0, 0, 0.1);
  }
}
</style>
