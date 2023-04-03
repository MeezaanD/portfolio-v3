<template>      
    <nav class="navbar navbar-expand-lg">
        <div class="container-fluid">
          <a class="navbar-brand" href="#home"><img src="https://i.postimg.cc/g224F76q/logo.png" style="height:7vh" alt=""></a>
          <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
          </button>
          <div class="collapse navbar-collapse" id="navbarSupportedContent">
            <ul class="navbar-nav ms-auto mb-2 mb-lg-0 gap-3">
              <li class="nav-item">
                <a class="nav-link" href="#home">Home</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="#about">About</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="#resume">Resume</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="#projects">Projects</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="#testimonials">Testimonials</a>
              </li>
              <li class="nav-item">
                <a class="nav-link" href="#contact">Contact</a>
              </li>
            </ul>
          </div>
        </div>
      </nav>
   
</template>
<script>
export default {
    
}
</script>
<style scoped>
    nav {
        width: 100%;
        color: transparent;
        border: 2px solid rgba(255,255,255,0.06);
        box-shadow: 0 10px 10px rgb(21, 48, 66);
        backdrop-filter: blur(10px);
        height: auto;
    }

    .navbar, .container {
        background-color: rgb(103, 172, 224);
    }

    .nav-link {
        font-family: 'Merienda', cursive;
        color: white;
        font-size:larger
    }
    .nav-link:hover {
        color: rgb(0, 44, 78);
    }


    
</style>