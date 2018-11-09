<template>
  <div class="overall">
    <div class="container">
  
      <h1>{{ msg }}</h1>
       
      <div class="row">
          <div class="section1 col-md-4">
              <h2 class="text-center"><countTo :startVal='startVal' :endVal='endVal1' :duration='3000'></countTo><sup>%</sup></h2>
              <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
          </div>
          <div class="section2 col-md-4">
              <h2 class="text-center"><countTo :startVal='startVal' :endVal='endVal2' :duration='3000'></countTo><sup>%</sup></h2>
              <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
          </div>
          <div class="section3 col-md-4">
              <h2 class="text-center"><countTo :startVal='startVal' :endVal='endVal3' :duration='3000'></countTo><sup>%</sup></h2>
              <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
          </div>
       </div>
       <div class="row">
         
      <button class="btn btn-primary mx-auto">Discover performance</button>
      
        </div>
    </div>
  </div>
</template>

<script>

import countTo from 'vue-count-to';


export default {
  name: 'Overall',
 
  components: { countTo },
  
  data () {
    return {
      msg: 'Overall success + growth',
      startVal: 0,
      endVal1: 12,
      endVal2: 75,
      endVal3: 28
    }
  }
 
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
    h1 {
        font-size: 2.246em;
        margin:48px 0px 30px;
    }
  h2 {
      font-size: 5.6em;
      border-bottom:1px solid #d8d8d8;
      margin-bottom:13px;
  }
  
  sup {
      font-size: 60%;
  }
  
  p {
      font-size:0.874em;
      line-height:1.3em;
  }
  
  .btn-primary {
    border-top:1px solid #002140;
    border-bottom:1px solid transparent;
    border-right:1px solid #002140;
    border-left:1px solid #002140;
    padding:18px;
    margin:26px auto 75px;
    background: transparent;
    color:#002140;
    text-transform:uppercase;
    font-size:0.874em;
    &:hover {
      background:#002140;
      color:#e6f0f3;
    }
  }

</style>