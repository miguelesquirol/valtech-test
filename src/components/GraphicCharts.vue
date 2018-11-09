<template>
  <div class="graphic">


<b-card no-body>
  <b-tabs pills card>
    <b-tab title="Lorem" active>
        <GChart   type="ColumnChart"
                  :data="chartData1"
                  :options="chartOptions"/>   
    </b-tab>
    <b-tab title="Ipsum">
      <GChart   type="ColumnChart"
                  :data="chartData2"
                  :options="chartOptions"/>   
    </b-tab>
    
    <b-tab title="Test 3">
      <GChart   type="ColumnChart"
                  :data="chartData3"
                  :options="chartOptions"/>   
    </b-tab>
    
  </b-tabs>
</b-card>



       
  </div>
</template>

<script>

import { GChart } from 'vue-google-charts'

export default {
  name: 'GraphicCharts',
 
  components: {
    GChart
  },
  
  data () {
    return {
   
      chartData1: [
        ['Year', 'Sales', 'Expenses', 'Profit'],
        ['2014', 1000, 400, 200],
        ['2015', 1170, 460, 250],
        ['2016', 660, 112, 300],
        ['2017', 1030, 540, 350]
      ],
      chartData2: [
        ['Year', 'Sales', 'Expenses', 'Profit'],
        ['2014', 100, 100, 200],
        ['2015', 170, 160, 250],
        ['2016', 460, 110, 300],
        ['2017', 930, 40, 350]
      ],
      chartData3: [
        ['Year', 'Sales', 'Expenses', 'Profit'],
        ['2014', 500, 430, 200],
        ['2015', 170, 460, 250],
        ['2016', 560, 1420, 300],
        ['2017', 3030, 540, 350]
      ],
      chartOptions: {
        chart: {
          title: 'Company Performance',
          subtitle: 'Sales, Expenses, and Profit: 2014-2017',
        }
      }
    }
  }
 
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    h3 {
        margin: 40px 0 0;
    }

    ul {
        list-style-type: none;
        padding: 0;
    }

    li {
        display: inline-block;
        margin: 0 10px;
    }

    a {
        color: #42b983;
    }
</style>
