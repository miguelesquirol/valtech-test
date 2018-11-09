<template>
  <div class="graphic">


       
      
<b-card no-body>
  <b-tabs pills card>
    <b-tab title="Lorem" active>
        <GChart
          :settings="{packages: ['bar']}"    
          :data="chartData"
          :options="chartOptions"
          :createChart="(el, google) => new google.charts.Bar(el)"
          @ready="onChartReady"
        />
  
    </b-tab>
    <b-tab title="Ipsum">
       <GChart
        :settings="{packages: ['bar']}"    
        :data="chartData2"
        :options="chartOptions"
        :createChart="(el, google) => new google.charts.Bar(el)"
        @ready="onChartReady"
      /> 
    </b-tab>
    
    <b-tab title="Test 3">
      <GChart
        :settings="{packages: ['bar']}"    
        :data="chartData3"
        :options="chartOptions"
        :createChart="(el, google) => new google.charts.Bar(el)"
        @ready="onChartReady"
      />  
    </b-tab>
    
  </b-tabs>
</b-card>



       
  </div>
</template>

<script>
import { GChart } from 'vue-google-charts'
export default {
  name: 'App',
  components: {
    GChart
  },
  data () {
    return {
      chartsLib: null, 
      // Array will be automatically processed with visualization.arrayToDataTable function
      
      
      chartData: [
        ['Year', 'Sales'],
        ['2013', 1000],
        ['2014', 1000],
        ['2015', 1170],
        ['2016', 660],
        ['2017', 1030],
        ['2018', 1030]
      ],
       chartData2: [
        ['Year', 'Sales'],
        ['2013', 1000],
        ['2014', 200],
        ['2015', 170],
        ['2016', 260],
        ['2017', 1230],
        ['2018', 1030]
      ],
       chartData3: [
        ['Year', 'Sales'],
        ['2014', 400],
        ['2015', 1470],
        ['2016', 560],
        ['2017', 30],
        ['2018', 1030]
      ]
      
    }
  },
  computed: {
    chartOptions () {
      if (!this.chartsLib) return null
      return this.chartsLib.charts.Bar.convertOptions({
        chart: {
          title: 'Company Performance',
        },
        bars: 'vertical', // Required for Material Bar Charts.
        hAxis: { format: 'decimal' },
        height: 200,
        colors: ['#e6ff00'],
        backgroundColor: '#002140',
        legend: {position: 'none'},
        titleTextStyle: {
            color: '#fff'
        },
        hAxis: {
            textStyle: {
                color: '#fff'
            },
            titleTextStyle: {
                color: '#fff'
            }
        },
        vAxis: {
            textStyle: {
                color: '#fff'
            },
            titleTextStyle: {
                color: '#fff'
            }
        },


      })
    }
  },
  methods: {
    onChartReady (chart, google) {
      this.chartsLib = google
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
    
    .card-body {
      margin:0px;
      padding:0px;
    }
    
   
</style>
