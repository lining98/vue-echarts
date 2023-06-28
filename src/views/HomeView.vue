<template>
  <div class="content bg">
    <dv-full-screen-container>
      <!-- 一行二等分 -->
      <div class="module-box">
        <div style="flex: 0 1 50%">
          <dv-border-box-8 style="width: 100%; height: 200px">
            <dv-capsule-chart
              :config="config"
              style="width: 100%; height: 200px"
            />
          </dv-border-box-8>
        </div>
        <div style="flex: 0 1 50%">
          <dv-border-box-3 style="width: 100%; height: 200px"
            >dv-border-box-3</dv-border-box-3
          >
        </div>
      </div>

      <div class="module-box">
        <div style="flex: 0 1 25%">
          <dv-border-box-9 style="width: 100%; height: 200px"
            >dv-border-box-3</dv-border-box-9
          >
          <dv-border-box-7 style="width: 100%; height: 200px"
            >dv-border-box-3</dv-border-box-7
          >
          <dv-border-box-2 style="width: 100%; height: 200px"
            >dv-border-box-3</dv-border-box-2
          >
        </div>
        <div style="flex: 0 1 50%">
          <dv-border-box-8 style="width: 100%; height: 600px"
            >dv-border-box-3</dv-border-box-8
          >
        </div>
        <div style="flex: 0 1 25%">
          <dv-border-box-1 style="width: 100%; height: 300px"
            >dv-border-box-3</dv-border-box-1
          >
          <dv-border-box-7 style="width: 100%; height: 300px"
            >dv-border-box-3</dv-border-box-7
          >
        </div>
      </div>

      <div class="module-box">
        <div style="flex: 0 1 70%">
          <dv-border-box-7 style="width: 100%; height: 200px"
            >dv-border-box-3</dv-border-box-7
          >
        </div>
        <div style="flex: 0 1 30%">
          <dv-border-box-9 style="width: 100%; height: 200px"
            >dv-border-box-3</dv-border-box-9
          >
        </div>
      </div>
    </dv-full-screen-container>
  </div>
</template>

<script>
export default {
  name: "HomeView",
  components: {},
  data() {
    return {
      config: {
        data: [
          {
            name: "南阳",
            value: 167,
          },
          {
            name: "周口",
            value: 67,
          },
          {
            name: "漯河",
            value: 123,
          },
          {
            name: "郑州",
            value: 55,
          },
          {
            name: "西峡",
            value: 98,
          },
        ],
        colors: ["#e062ae", "#fb7293", "#e690d1", "#32c5e9", "#96bfff"],
        unit: "单位",
        showValue:true
      },
    };
  },
};
</script>

<style scoped>
.content {
  background: #010d39;
  color: #ffffff;
  height: 100vh;
  display: flex;
}
.module-box {
  display: flex;
  margin: 10px;
}
</style>
