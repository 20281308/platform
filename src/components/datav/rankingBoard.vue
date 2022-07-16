<template>
  <div id="ranking-board">
    <div class="ranking-board-title">各车厢完成情况</div>
    <div></div>
    <dv-scroll-ranking-board :config="config" />
  </div>
</template>

<script>
export default {
  name: 'RankingBoard',
  data () {
    return {
      config: {
        data: [
          {
            name: '1号车厢',
            value: 95
          },
          {
            name: '2号车厢',
            value: 90
          },
          {
            name: '3号车厢',
            value: 98
          },
          {
            name: '4号车厢',
            value: 96
          },
          {
            name: '5号车厢',
            value: 90
          },
          {
            name: '6号车厢',
            value: 95
          },
          {
            name: '7号车厢',
            value: 99
          },
          {
            name: '8号车厢',
            value: 99
          },
          {
            name: '9号车厢',
            value: 99
          },
          {
            name: '10号车厢',
            value: 99
          },
          {
            name: '11号车厢',
            value: 92
          },
          {
            name: '12号车厢',
            value: 94
          },
          {
            name: '13号车厢',
            value: 93
          },
          {
            name: '14号车厢',
            value: 89
          },
          {
            name: '15号车厢',
            value: 94
          },
          {
            name: '16号车厢',
            value: 91
          },
          
        ],
        rowNum: 20
      }
    }
  }
}
</script>

<style lang="less">
#ranking-board {
  width: 15%;
  box-shadow: 0 0 3px blue;
  display: flex;
  flex-direction: column;
  background-color: rgba(6, 30, 93, 0.5);
  border-top: 2px solid rgba(1, 153, 209, .5);
  box-sizing: border-box;
  padding: 0px 30px;

  .ranking-board-title {
    font-weight: bold;
    height: 50px;
    display: flex;
    align-items: center;
    font-size: 20px;
  }

  .dv-scroll-ranking-board {
    flex: 1;
  }
}
</style>
