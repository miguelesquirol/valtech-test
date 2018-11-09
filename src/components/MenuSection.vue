<template>
  <div class="menu">
      
       <nav class="navbar nav-secondary navbar-expand-lg navbar-dark bg-dark">
            <div class="container justify-content-end">
              <div class="collapse navbar-collapse ">
                <ul class="navbar-nav">
                  <li class="nav-item"><a href="#" target="_blank" rel="noopener" class="nav-link">Research</a></li>
                  <li class="nav-item"><a href="#" target="_blank" rel="noopener" class="nav-link">Locations</a></li>
                  <li class="nav-item"><a href="#" target="_blank" rel="noopener" class="nav-link">Contributions</a></li>
                  <li class="nav-item"><a href="#" target="_blank" rel="noopener" class="nav-link">News hub</a></li>
                </ul>
                <ul class="navbar-nav lang">
                  <li><a href="#" target="_blank" rel="noopener">FR</a></li>
                </ul> 
             </div>
         </div>
        </nav>
      
<b-navbar toggleable="md" type="dark" variant="info" class="navbar nav-secondary navbar-expand-lg navbar-dark bg-dark">
    <div class="container">

      <b-navbar-brand href="#">NavBar</b-navbar-brand>
    
      <b-navbar-toggle target="nav_collapse"></b-navbar-toggle>
    
    
      <b-collapse is-nav id="nav_collapse" class="justify-content-end">
    
        <b-navbar-nav >
      
           <b-nav-item href="#" class="nav-item active"><a href="#" target="_blank" rel="noopener" class="nav-link">We are ipsu <span class="sr-only">(current)</span>m</a></b-nav-item>
           <b-nav-item href="#" target="_blank" rel="noopener" class="nav-link">We are dolr</a></b-nav-item>
           <b-nav-item href="#" target="_blank" rel="noopener" class="nav-link">iopsum</a></b-nav-item>
           <b-nav-item href="#" target="_blank" rel="noopener" class="nav-link">amet</a></b-nav-item>
                      
                      
        </b-navbar-nav>
    
        <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto">
    
        
    
          
    
      
        </b-navbar-nav>
    
      </b-collapse>
  </div>

</b-navbar>    


       
        
    
  </div>
</template>

<script>
    export default {
        name: 'MenuSection'
    }
</script>


<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.menu {
    margin:0px;
    padding:0px;
}
.nav-secondary {
    margin:0px;
    padding:0px;
    
    li {
        text-transform:uppercase;
        font-size:0.624em;
        padding:10px 17px;
        margin:0px;
        a {
        margin:0px;
        padding:0px;
        }
    }
    
    .lang {
        border-left:1px solid rgba(255,255,255,0.3);
        a {color:#fff;}
    }
}

.navbar-collapse {
    flex-grow:0;
}
.nav-main {
    
    li {
        font-weight:900;
        font-size: 0.874em;
        padding:0px 17px;

        &.active a {
            opacity:0.4; 
        }
    }
}
</style>
