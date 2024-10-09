<template>
  <div
    class="control"
    id="capsule-chart">
    <div class="title-text">{{ config.title }}</div>
    <dv-capsule-chart
      :config="config"
      style="width: 500px; height: 300px" />
  </div>
</template>

<script>
export default {
  name: "capsuleChart",
  data() {
    return {
      config: {
        title: "胶囊柱图",
        data: [
          {
            name: "南阳",
            value: 167,
          },
          {
            name: "周口",
            value: 123,
          },
          {
            name: "漯河",
            value: 98,
          },
          {
            name: "郑州",
            value: 75,
          },
          {
            name: "西峡",
            value: 66,
          },
        ],
        colors: ["#e062ae", "#fb7293", "#e690d1", "#32c5e9", "#96bfff"],
        unit: "例",
        showValue: true,
      },
    };
  },
};
</script>
