<template>
  <div class="timeline">
      
    <h1>{{ msg }}</h1>
     
     
     
        
    
    <b-card no-body>
      <b-tabs pills card>
        <b-tab title="1998">
          <h2>1998 ipsum projection lorem</h2>
          <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut nim ad minim veniam</p>
          <p>Quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat</p>
          </p>
        </b-tab>
        <b-tab title="2002" active>
          <h2>2002 ipsum projection lorem</h2>
          <div class="row">
            <div class="col-md-4">
               <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut nim ad minim veniam</p>
               <p>Quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat</p>
            </div>
            <div class="col-md-4">
              <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut nim ad minim veniam</p>
              <p>Quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat</p>
            </div>
            <div class="col-md-4">
              <GraphicCharts></GraphicCharts>
            </div>

          </div>
          
        </b-tab>
        <b-tab title="2006">
          <h2>2006 ipsum projection lorem</h2>
          <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut nim ad minim veniam</p>
          <p>Quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat</p>
          </p>
        </b-tab>
        <b-tab title="2012">
          <h2>2012 ipsum projection lorem</h2>
          <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut nim ad minim veniam</p>
          <p>Quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat</p>
          </p>
        </b-tab>
        <b-tab title="2014">
          <h2>2014 ipsum projection lorem</h2>
          <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut nim ad minim veniam</p>
          <p>Quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat</p>
          </p>
        </b-tab>
        <b-tab title="2018">
          <h2>2018 ipsum projection lorem</h2>
          <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut nim ad minim veniam</p>
          <p>Quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat</p>
          </p>
        </b-tab>
        
      </b-tabs>
    </b-card>

  </div>
</template>

<script>

import GraphicCharts from './GraphicCharts.vue'


export default {
  name: 'Timeline',

  data () {
    return {
      msg: 'Timeline of success',
    }
  },
   components:{
      GraphicCharts
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

  $dark: #002140;

  .timeline, .card {
    background: $dark;
  }
  
  h1 {
    color: #fff;
    font-size: 2.246em;
    padding:44px 0px 38px;
    
  }
  
  p {
    color:#fff;
    font-size:0.998em;
    line-height: 1.498em;
  }
  
  h2 {
    color: #e6ff00;
  }

 
  li.nav-item {
    background: #fff !important;
}


</style>
