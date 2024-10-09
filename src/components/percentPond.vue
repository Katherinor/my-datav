<template>
  <div
    class="control"
    id="percent-pond">
    <div class="title-text">{{ config.title }}</div>
    <dv-percent-pond
      :config="config"
      style="width: 500px; height: 300px" />
  </div>
</template>

<script>
export default {
  name: "percentPond",
  data() {
    return {
      config: {
        title: "进度池",
        value: 86,
      },
    };
  },
};
</script>
