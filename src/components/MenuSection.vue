<template>
  <div class="menu">
      
    <nav class="navbar nav-secondary navbar-expand-lg navbar-dark bg-dark">
      <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
    
      <div class="collapse navbar-collapse justify-content-end">
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
     
    </nav>

    <nav class="navbar nav-main navbar-expand-md navbar-dark bg-dark"  id="navbarSupportedContent">
        <a href="/" class="navbar-brand">Bootstrap 4</a>
        <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbar7">
            <span class="navbar-toggler-icon"></span>
        </button>
        <div class="navbar-collapse collapse justify-content-stretch" id="navbar7">
            <ul class="navbar-nav ml-auto">
                 <li class="nav-item active"><a href="#" target="_blank" rel="noopener" class="nav-link">We are ipsu <span class="sr-only">(current)</span>m</a></li>
              <li><a href="#" target="_blank" rel="noopener" class="nav-link">We are dolr</a></li>
              <li><a href="#" target="_blank" rel="noopener" class="nav-link">iopsum</a></li>
              <li><a href="#" target="_blank" rel="noopener" class="nav-link">amet</a></li>
            </ul>
        </div>
    </nav>

     
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
