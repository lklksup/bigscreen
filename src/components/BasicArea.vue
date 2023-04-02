<template>
  <div ref="chart" style="width: 320px; height: 250px"></div>
</template>

<script>
import * as echarts from "echarts";

export default {
  name: "BasicArea",
  props: {
    option: { type: Object, default: null },
  },
  data() {
    myChart:null
  },
  created() {},
  mounted() {
    this.myChart = echarts.init(this.$refs.chart);
    this.myChart.setOption(this.option);
    console.log("这是组件中的this")
    console.log(this)
  },
};
</script>
