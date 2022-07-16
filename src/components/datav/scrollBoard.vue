<template>
  <div id="scroll-board">
    <dv-scroll-board :config="config" />
  </div>
</template>

<script>
export default {
  name: 'ScrollBoard',
  data () {
    return {
      config: {
        header: ['时间', '处理信息'],
        data: [
          [' 09:25', '70摄氏度,含水率为10%,可进行造粒'],
          [' 10:25', '调节ph在9左右,投加氯化镁'],
          [' 11:25', '紫外线灯管消毒'],
          [' 12:25', '70摄氏度,含水率为10%,可进行造粒'],
          [' 13:25', '调节ph在9左右,投加氯化镁'],
          [' 14:25', '紫外线灯管消毒'],
          [' 15:25', '70摄氏度,含水率为10%,可进行造粒'],
          [' 16:25', '经过疫情中风险地区,调整清洁水比例'],
          [' 17:25', '采集数据,上传到云端'],
          [' 18:25', '活性炭吸附污染物不达标,提醒更换']
        ],
        index: true,
        columnWidth: [50, 60, 300],
        align: ['center'],
        rowNum: 6,
        headerBGC: '#1981f6',
        headerHeight: 45,
        oddRowBGC: 'rgba(0, 44, 81, 0.8)',
        evenRowBGC: 'rgba(10, 29, 50, 0.8)'
      }
    }
  }
}
</script>

<style lang="less">
#scroll-board {
  width: 35%;
  box-sizing: border-box;
  margin-left: 20px;
  margin-right: 10px;
  height: 100%;
  overflow: hidden;
}
</style>
