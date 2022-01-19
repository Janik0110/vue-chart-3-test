<script setup lang="ts">
import { LineChart, useLineChart } from 'vue-chart-3';

const {lineChartProps} = useLineChart({
  chartData: {
    labels:[1,2,3],
    datasets: [
      {
        label: 'My First dataset',
        backgroundColor: '#f87979',
        data: [10, 20, 30]
      }
    ]
  }
})
</script>

<template>
  <LineChart v-bind="lineChartProps" />
</template>

