<template>
  <div id="app">
    <div class="component-container">
      <activeRingChart />
      <capsuleChart />
      <waterLevelPond />
      <percentPond />
      <flylineChartEnhanced />
      <conicalColumnChart />
      <digitalFlop />
      <scrollBoard />
      <scrollRankBoard />
    </div>
  </div>
</template>

<script>
import scrollRankBoard from "./components/scrollRankBoard.vue";
import scrollBoard from "./components/scrollBoard.vue";
import digitalFlop from "./components/digitalFlop.vue";
import conicalColumnChart from "./components/conicalColumnChart.vue";
import flylineChartEnhanced from "./components/flylineChartEnhanced.vue";
import percentPond from "./components/percentPond.vue";
import waterLevelPond from "./components/waterLevelPond.vue";
import capsuleChart from "./components/capsuleChart.vue";
import activeRingChart from "./components/activeRingChart.vue";
import Charts from "@jiaminghi/charts";
const container = document.getElementById("app");

const myChart = new Charts(container);
myChart.setOption({
  title: "My Chart",
  // ...otherConfig
});

export default {
  name: "App",
  components: {
    scrollRankBoard,
    scrollBoard,
    digitalFlop,
    conicalColumnChart,
    flylineChartEnhanced,
    percentPond,
    waterLevelPond,
    capsuleChart,
    activeRingChart,
  },
  mounted() {
    console.log("奇迹发生了！");
  },
};
</script>

<style>
* {
  margin: 0;
  padding: 0;
}
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  background-color: #5cb85c;
  display: flex;
  justify-content: center;
  align-items: center;
}

.component-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 20px; /* 间距 */
}

.component-container > * {
  flex: 0 0 45%;
  display: flex;
  justify-content: center;
  align-items: center;
}

.control {
  margin: 0 0 20px 0;
}
</style>
