<template>
  <div
    class="control"
    id="active-ring-chart">
    <div class="title-text">{{ config.title }}</div>
    <dv-active-ring-chart
      :config="config"
      style="width: 500px; height: 300px" />
  </div>
</template>

<script>
export default {
  name: "activeRingChart",
  data() {
    return {
      config: {
        title: "动态环图",
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
            value: 78,
          },
          {
            name: "驻马店",
            value: 66,
          },
          {
            name: "新乡",
            value: 80,
          },
        ],
      },
    };
  },
};
</script>
