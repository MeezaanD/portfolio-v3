<template>
    <div id="projects">
        <h6 class="heading">Projects</h6>
        <h4 class="text-center">My Latest Work</h4> 
           <div class="row gap-3 p-3">
                <div  data-aos="zoom-out-up" class="container" v-for="item in projects" :key="item">
                <img :src="item.image" class="image">
                <div class="overlay">
                    <div class="text">
                        <h3>{{ item.name }}</h3>
                        <p>{{ item.language }}</p>
                        <p>{{ item.desc }}</p>
                        
                          <br><br> 
                            <div class="btn-group">
                              <a :href="item.github" target="_blank" class="btn btn-outline-dark"><i class="fa-brands fa-github"></i></a>
                              <a :href="item.live" target="_blank" class="btn btn-outline-dark"><i class="fa-brands fa-chrome"></i></a>
                    </div>
                      </div>
                  
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
        name: 'First Portfolio',
        desc: 'This was my first Portfolio built with HTML & CSS',
        image:"https://i.postimg.cc/yxq1dGF1/7fcf815a55c64fe566302fa4f0037095.webp",
        github: "https://github.com/MeezaanD/Portfolio.git",
        live: "https://phenomenal-semolina-67d782.netlify.app/"
    },
    {
        language: 'Vue 3 & Node Js',
        name: 'Active8',
        desc: 'This was my first fullstack project built with my peer Cassidy Lawrence working on the backend',
        image: "https://i.postimg.cc/1RFg1tr8/activ8.png" ,
        github: "https://github.com/CassidyRomarioLawrence/Activ8_nodeEOMP",
        live: "https://activ8-fullstack.web.app"
    },
    {
        language: 'HTML, Bootstrap',
        name: 'Ecommerce Website',
        desc: 'Home page built using bootstrap for the first time',
        image:"https://i.postimg.cc/zBPkYsHJ/14d87a3887139e044ed629ae32107c1e.jpg",
        github: "https://github.com/MeezaanD/Ecommerce-Project.git",
        live: "https://ecomprojectmeezaan.netlify.app/"
    },
    {
      language: 'HTML, CSS, Javascript',
      name: 'Calculator App',
      desc: 'Basic calculator built with HTML, CSS & Javascript',
      image: "https://i.postimg.cc/4y5DrRMV/calculator.png",
      github: "https://github.com/MeezaanD/Calculator-TEST-.git",
      live: "https://calculator-md240503.netlify.app"
    },
    {
        language: 'HTML, CSS, Javascript',
        name: 'Point of Sales',
        desc: 'Ecommerce website built with a cart and checkout system',
        image: "https://i.postimg.cc/GmZCjcMY/Grey-Apple-IDi-PAd.png",
        github: "https://github.com/MeezaanD/MD-POS.git",
        live: "https://meezaanpointofsales.netlify.app"
      },
      {
        language: 'Vue',
        name: 'Mini-Project',
        desc: 'Basic home page design of a Mercedes Website',
        image: "https://i.postimg.cc/3R6GzfMP/download.jpg",
        github: "https://github.com/MeezaanD/Mini-Project.git",
        live: "https://miniprojectmeezaan.netlify.app/"
      }, 
      {
        language: 'Vue JS, Node JS, MySQL',
        name: 'Nightcrawler',
        desc: 'FullStack Ecommerce Capstone Project',
        image: "https://i.postimg.cc/Z0kmQ4WF/NC2.png",
        github: "https://github.com/MeezaanD/Capstone-project",
        live: "https://nightcrawler-9e9da.web.app/"
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
    font-size: 15px;
    position: absolute;
    top: 50%;
    left: 50%;
    -webkit-transform: translate(-50%, -50%);
    -ms-transform: translate(-50%, -50%);
    transform: translate(-50%, -50%);
  }


</style>