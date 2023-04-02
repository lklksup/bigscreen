<template>
  <div class="content bg">
    <!-- 全屏容器 -->
    <dv-full-screen-container>
      <div class="header">
        <dv-decoration-10 style="width: 25%; height: 5px" />
        <dv-decoration-8 style="width: 300px; height: 50px; margin-top: 5px" />
        <dv-decoration-11 style="width: 200px; height: 60px"
          >可视化大屏项目模拟</dv-decoration-11
        >
        <dv-decoration-8
          :reverse="true"
          style="width: 300px; height: 50px; margin-top: 5px"
        />
        <dv-decoration-10 :reverse="true" style="width: 25%; height: 5px" />
      </div>
      <div class="module-box">
        <div style="flex: 0 1 25%">
          <dv-border-box-13 style="width: 100%; height: 200px">
            <div class="container">
              <!-- <BasicArea ></BasicArea> -->
            </div>
          </dv-border-box-13>
          <dv-border-box-1 style="width: 100%; height: 200px"
            ><div class="container">
              </div
          ></dv-border-box-1>
          <dv-border-box-2 style="width: 100%; height: 200px"
            ><div class="container">
              <!-- <BasicArea ></BasicArea> -->
              </div
          ></dv-border-box-2>
        </div>
        <div style="flex: 0 1 50%">
          <dv-border-box-12 style="width: 100%; height: 600px"
            >dv-border-box-3</dv-border-box-12
          >
        </div>
        <div style="flex: 0 1 25%">
          <dv-border-box-1 style="width: 100%; height: 200px"
            >dv-border-box-3</dv-border-box-1
          >
          <dv-border-box-8 style="width: 100%; height: 400px"
            >智障</dv-border-box-8
          >
        </div>
      </div>
    </dv-full-screen-container>
  </div>
</template>

<script>
// @ is an alias to /src
import BasicArea from "@/components/BasicArea.vue";
export default {
  name: "HomeView",
  components: {
    BasicArea,
  },
  data() {
    arr1: [820, 932, 901, 934, 1290, 1330, 1320];
    arr2: [820, 932, 901, 934, 1290, 1330, 1320];
    arr3: [820, 932, 901, 934, 1290, 1330, 1210];
  },

  methods: {},
};
</script>

<style scoped>
* {
  margin: 0;
  padding: 0;
}
html {
  -webkit-text-size-adjust: 100%;
  -ms-text-size-adjust: 100%;
  font-size: 62.5%;
}

body,
input,
button,
a,
textarea,
select {
  margin: 0;
  font-family: "Helvetica Neue", Helvetica, "Hiragino Sans GB";
  font-size: 1.4rem;
  line-height: 1.5;
  color: #333;
}

html,
body {
  width: 100%;
  height: 100%;
  margin: 0;
}

a {
  text-decoration: none;
}

a:hover,
a:focus {
  text-decoration: none;
}

a:hover {
  filter: alpha(opacity=90);
  opacity: 0.9;
}

.content {
  color: #fff;
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100vh;
}

.bg {
  background: url("../assets/images/bg.png") no-repeat center;
  background: cover;
}

.module-box {
  display: flex;
  justify-content: space-between;
}

.header {
  width: 100%;
  height: 70px;
  margin-top: 10px;
  display: flex;
  justify-content: center;
}

.container {
  width: 100%;
  height: 100%;

  display: flex;
  justify-content: center;
  align-items: center;
}
</style>

