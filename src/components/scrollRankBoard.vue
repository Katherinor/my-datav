<template>
  <div
    class="control"
    id="scroll-ranking-board">
    <div class="title-text">{{ config.title }}</div>
    <dv-scroll-ranking-board
      :config="config"
      style="width: 500px; height: 300px" />
  </div>
</template>

<script>
export default {
  name: "scrollRankBoard",
  data() {
    return {
      config: {
        title: "排名轮播图",
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
          {
            name: "信阳",
            value: 45,
          },
          {
            name: "漯河",
            value: 29,
          },
        ],
        unit: "马赫",
      },
    };
  },
};
</script>

<style></style>
