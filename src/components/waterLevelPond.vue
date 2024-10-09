<template>
  <div
    class="control"
    id="water-level-pond">
    <div class="title-text">{{ config.title }}</div>
    <dv-water-level-pond
      :config="config"
      style="width: 500px; height: 300px" />
  </div>
</template>

<script>
export default {
  name: "waterLevelPond",
  data() {
    return {
      config: {
        title: "水位池",
        data: [36],
      },
    };
  },
};
</script>
