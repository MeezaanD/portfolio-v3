<template>
    <div id="projects">
        <h6 class="heading">Projects</h6>
        <h4 class="text-center">My Latest Work</h4> 
           <div class="row gap-3 p-3">
                <div class="container" v-for="item in projects" :key="item">
                <img :src="item.image" class="image">
                <div class="overlay">
                  <h3 class="text">{{ item.name }}
                    <br><br> 
                      <div class="btn-group">
                        <a :href="item.github" target="_blank" class="btn btn-outline-dark">Github</a>
                        <a :href="item.live" target="_blank" class="btn btn-outline-dark">Live </a>
                      </div>
                  </h3>
           </div>
            </div>
          </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
     projects : [
    {
        language: 'HTML & CSS',
        name: 'Portfolio',
        image:"https://i.postimg.cc/mDwG2M4Q/first-Porfolio.png",
        github: "https://github.com/MeezaanD/Portfolio.git",
        live: "https://phenomenal-semolina-67d782.netlify.app/"
    },
    {
        language: 'Vue 3 & Node Js',
        name: 'Active8',
        image: "https://i.postimg.cc/Bv2Q7z9B/active.png" ,
        github: "https://github.com/CassidyRomarioLawrence/Activ8_nodeEOMP",
        live: "https://activ8-fullstack.web.app"
    },
    {
        language: 'HTML & CSS',
        name: 'Ecommerce Website',
        image:"https://i.postimg.cc/rpR1kCSP/ecommerce.png",
        github: "https://github.com/MeezaanD/Ecommerce-Project.git",
        live: "https://ecomprojectmeezaan.netlify.app/"
    },
    {
      language: 'HTML, CSS, Javascript',
      name: 'Calculator App',
      image: "https://i.postimg.cc/4y5DrRMV/calculator.png",
      github: "https://github.com/MeezaanD/Calculator-TEST-.git",
      live: "https://calculator-md240503.netlify.app"
    },
    {
        language: 'HTML, CSS, Javascript',
        name: 'Point of Sales',
        image: "https://i.postimg.cc/L5YYzyhk/pos.png",
        github: "https://github.com/MeezaanD/MD-POS.git",
        live: "https://meezaanpointofsales.netlify.app"
      },
      {
        language: 'Vue',
        name: 'Mini-Project',
        image: "https://i.postimg.cc/prPWhHn1/mini.png",
        github: "https://github.com/MeezaanD/Mini-Project.git",
        live: "https://miniprojectmeezaan.netlify.app/"
      }
  ], 
    }
}
}
</script>

<style scoped>
#projects {
    background-image: linear-gradient(rgb(103, 172, 224), white);
    height: auto;
}

.container {
    position: relative;
    width: auto;
  }
  
  .image {
    display: flex;
    width: 100%;
    height: 20rem;
  }
  
  .overlay {
    position: absolute;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    height: 100%;
    width: 100%;
    opacity: 0;
    transition: .5s ease;
    background: rgba(90, 90, 90, 0.5);
    backdrop-filter: blur(50px);
    overflow: hidden;
  }
  
  .container:hover .overlay {
    opacity: 1;
  }
  
  .text {
    color: white;
    font-family: 'Merienda', cursive;
    font-size: 20px;
    position: absolute;
    top: 20%;
    left: 50%;
    -webkit-transform: translate(-50%, -50%);
    -ms-transform: translate(-50%, -50%);
    transform: translate(-50%, -50%);
  }


</style>