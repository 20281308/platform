<template>
  <div id="air-level-chart">
    <div class="air-level-chart-title">空气消杀率</div>


    <div class="chart-container">
      <dv-water-level-pond :config="config" />
    </div>
  </div>
</template>

<script>
export default {
  name: 'WaterLevelChart',
  data () {
    return {
      config: {
        data: [95],
        shape: 'round',
        waveHeight: 25,
        waveNum: 2
      }
    }
  }
}
</script>

<style lang="less">
#air-level-chart {
  width: 20%;
  box-sizing: border-box;
  margin-left: 20px;
  background-color: rgba(6, 30, 93, 0.5);
  border-top: 2px solid rgba(1, 153, 209, .5);
  display: flex;
  flex-direction: column;

  .air-level-chart-title {
    font-weight: bold;
    height: 50px;
    display: flex;
    align-items: center;
    font-size: 20px;
    justify-content: center;
  }

//   .air-level-chart-details {
//     height: 15%;
//     display: flex;
//     justify-content: center;
//     font-size: 50px;
//     align-items: flex-end;

//     span {
//       font-size: 35px;
//       font-weight: bold;
//       color: #58a1ff;
//       margin: 0 5px;
//       margin-bottom: -5px;
//     }
//   }

  .chart-container {
    flex: 1;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .dv-water-pond-level {
    max-width: 90%;
    width: 200px;
    height: 200px;
    border: 10px solid #19c3eb;
    border-radius: 50%;

    ellipse {
      stroke: transparent !important;
    }

    text {
      font-size: 40px;
    }
  }
}
</style>
