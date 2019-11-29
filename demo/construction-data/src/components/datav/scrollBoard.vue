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
        header: ['时间', '预警信息', '状态', '产线'],
        data: [
          ['2019-11-01 19:25:00', '产线报停-物料缺失', '未响应', '产线一'],
          ['2019-11-02 17:25:00', '产线报停-设备异常', '处理中', '产线二'],
          ['2019-11-03 16:25:00', '生产计划-计划变更', '处理中', '产线三'],
          ['2019-11-04 15:25:00', '物料配送-通用物料', '未响应', '产线四'],
          ['2019-11-05 14:25:00', '物料配送-通用物料', '未响应', '产线五'],
          ['2019-11-06 13:25:00', '产线报停-物料不合格', '未响应', '产线六'],
          ['2019-11-08 11:25:00', '生产计划-计划变更', '处理中', '产线七'],
          ['2019-11-07 12:25:00', '产线报停-质检不合格', '处理中', '产线八'],
          ['2019-11-09 10:25:00', '物料配送-物料不合格', '未响应', '产线九'],
          ['2019-11-10 09:25:00', '物料配送-物料不合格', '处理中', '产线十']
        ],
        index: true,
        columnWidth: [50, 170, 300],
        align: ['center'],
        rowNum: 7,
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
  width: 50%;
  box-sizing: border-box;
  margin-left: 20px;
  height: 100%;
  overflow: hidden;
}
</style>
