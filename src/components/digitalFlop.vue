<template>
  <div
    class="control"
    id="digital-flop">
    <div class="digitalFlopTitle">
      <div class="title-text">{{ config.title }}</div>
      <el-button
        class="btn"
        @click="randomizeNumber">
        随机数字
      </el-button>
    </div>
    <dv-digital-flop
      :config="config"
      style="width: 500px; height: 300px" />
  </div>
</template>

<script>
export default {
  name: "digitalFlop",
  data() {
    return {
      config: {
        title: "数字翻牌器",
        number: [100],
        toFixed: 2,
        content: "Lv.{nt}",
      },
    };
  },
  methods: {
    randomizeNumber() {
      const randomNumForNumber = Number((Math.random() * 10000).toFixed(2));
      this.config = {
        ...this.config,
        number: [randomNumForNumber],
      };
    },
  },
};
</script>

<style lang="less">
.digitalFlopTitle {
  display: flex;
  align-items: center;
  .btn {
    margin-left: 20px;
  }
}
</style>
