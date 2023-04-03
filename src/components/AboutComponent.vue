<template>
    <div id="about">
        <h6 class="heading">About</h6>
            <div class="container">
                <div class="row align-items-center">
                  <div data-aos="fade-right" class="col-sm-6">
                    <img class="img-fluid" src="https://i.postimg.cc/d3Yjj506/test.jpg" alt="">
                  </div>
                  <div  data-aos="fade-up" class="col-sm-6 align-self-start" style="padding-left: 30px">
                    <h2>About Me</h2>
                    <p>Hello, my name is Meezaan Davids I am 19 years old, and I was born in Cape Town South Africa. I would like to think I am a genuine straight forward person. I am very interested in learning new skills, whether it is cooking or coding I am very much interested in it. I would also like to consider myself a very passionate sports fan. I try to keep up to date with all my sports. I am really interested in a possible career in web design. At this point in my life I am very into learning new things because new experiences bring new opportunities.</p>
                    <div class="container text-start">
                        <div class="row align-self-start">
                          <div class="col-sm-6">
                                <b>FullName</b>  Meezaan Davids <br>
                                <b>D.O.B</b> 24/05/03 <br>
                                <b>Gender</b> Male <br>
                                <b>Citizenship</b> South African
                          </div>
                        </div>
                        <br>
                        <div class="btn-group" role="group" aria-label="Basic outlined example">
                          <a href="#" type="button" class="btn btn-outline-primary">CV</a>
                          <a href="#contact" type="button" class="btn btn-outline-primary">Let's talk</a>
                        </div>
                      </div>
                      
                  
                  </div>
                </div>
              </div>
    </div>
</template>

<script>

export default {

}

</script>



<style scoped>

#about {
    background-image: linear-gradient(rgb(103, 172, 224), white);
    height: auto;
}

.container {
    justify-content: center;
    position: relative;
    display: block;
    margin: auto;
}
.img-fluid {
    width: auto; 
    background-color: transparent;
    border: 1px solid white;
    border-radius: 5px;
    box-shadow: 0 20px 30px rgba(0,0,0,0.2);
    backdrop-filter: blur(10px); 
    transition: all 0.3s;
    transform: scale(1);
}

.img-fluid:hover {
    transform: scale(1.1);
  }

h2, b {
    font-family: 'Merienda', cursive;
}

p {
    font-size: large;
}




</style>