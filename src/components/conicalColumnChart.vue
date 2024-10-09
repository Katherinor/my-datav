<template>
  <div
    class="control"
    id="conical-column-chart">
    <div class="title-text">{{ config.title }}</div>
    <dv-conical-column-chart
      :config="config"
      style="width: 500px; height: 300px" />
  </div>
</template>

<script>
export default {
  name: "conicalColumnChart",
  data() {
    return {
      config: {
        title: "锥形柱图",
        data: [
          {
            name: "周口",
            value: 55,
          },
          {
            name: "南阳",
            value: 120,
          },
          {
            name: "西峡",
            value: 71,
          },
          {
            name: "驻马店",
            value: 66,
          },
          {
            name: "新乡",
            value: 80,
          },
          {
            name: "信阳",
            value: 35,
          },
          {
            name: "漯河",
            value: 15,
          },
        ],
      },
    };
  },
};
</script>
