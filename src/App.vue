<template>
  <div id="app">
      <MenuSection></MenuSection>
      <Overall></Overall>
      <Timeline></Timeline>
  </div>
</template>

<script>
import 'babel-polyfill'
import MenuSection from './components/MenuSection.vue'
import Overall from './components/Overall.vue'
import Timeline from './components/Timeline.vue'



export default {
  name: 'app',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
  components:{
      MenuSection,
      Overall,
      Timeline
  },
}
</script>

<style lang="scss">
  $dark: #002140;
  $body-bg: #e6f0f3;
  $font-family-sans-serif:  "Arial";
  $grid-gutter-width: 40px;
  $navbar-dark-color: #fff;
  $btn-border-radius: 0;
  $nav-pills-link-active-bg: #e6ff00;
  $nav-pills-link-active-color:$dark;
  $nav-pills-border-radius: 0;
  
  .graphic {
    .tab-pane {
      overflow:hidden;
    }
  }
  
  .graphic {
    .card {        
      border:0px solid transparent;
      }
    .card-header {
        border:0px solid transparent;
        background:$dark;
        position:relative;
        z-index:2;
        
         &:after {
         display:none;
        }
        .nav-pills {
          display:flex;
          justify-content: space-between;
          position:relative;
          z-index:20;
         
        }
        .nav-item:nth-child(1) {
          border: 1px solid #e6ff00;
          position:relative;
          a {
            color:#fff;
            padding:3px 10px;
            background:$dark;
            font-size:0.624em;
            &:hover {
             color:$dark;
             background: #e6ff00;
             }
          }
        .active  {
          color:$dark;
          background: #e6ff00;
        }
      }
      .nav-item:nth-child(3) {
          border: 1px solid #ffa32b;
          position:relative;
          a {
            color:#ffa32b;
            padding:3px 10px;
            background:$dark;
            font-size:0.624em;
            &:hover {
             color:$dark;
             background: #ffa32b;
             }
          }
        .active  {
          color:$dark;
          background: #ffa32b;
        }
      }
      .nav-item:nth-child(2) {
          border: 1px solid #61e3e8;
          position:relative;
          a {
            color:#61e3e8;
            padding:3px 10px;
            background:$dark;
            font-size:0.624em;
            &:hover {
             color:$dark;
             background: #61e3e8;
             }
          }
        .active  {
          color:$dark;
          background: #61e3e8;
        }
      }
    }
  }

  .timeline {
    .card {        
      border:0px solid transparent;
      }
    .card-header {
        border:0px solid transparent;
        background:$dark;
        position:relative;
        z-index:2;
        
         &:after {
          content: '';
          width: 100%;
          border-bottom: solid 1px #d6d6d6;
          position: absolute;
          left: 0;
          top: 50%;
          z-index: 1;
        }
        .nav-pills {
          display:flex;
          justify-content: space-between;
           position:relative;
        z-index:20;
         
        }
        .nav-item {
          border: 1px solid #fff;
          position:relative;
          a {
            color:#fff;
            padding:3px 10px;
            background:$dark;

              &:hover {
                 color:$dark;
                 background: #e6ff00;
              }
            }
          .active  {
            color:$dark;
            background: #e6ff00;
            }
          }
       }
  }
  @import "~bootstrap/scss/bootstrap"; 
  
</style>
