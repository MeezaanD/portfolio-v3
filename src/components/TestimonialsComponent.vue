<template>
    <div id="testimonials">
        <h6 class="heading">Testimonials</h6>
        <div class="testimonials text-center">
              <div class="row" style="gap: 2rem">
                    <div v-for="item in info" :key="item" class="card text-center">
                        <i class="fa fa-quote-left fa-3x card-img-top rounded-circle" aria-hidden="true"></i>
                      <img :src="item.image" data-aos="zoom-in" style="height: 100%;width: 100%;border-radius: 50%;padding: 20px;" class="image-fluid">
                    <div class="overlay">
                      <div class="text">
                          <cite title="Source Title"><b>{{ item.name }}</b></cite>
                          <br>
                          <h4>{{ item.reference }}</h4>
                          <div class="card-body blockquote">
                            <p class="card-text">{{ item.message }}</p>
                          </div>
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
            info : [
                {
                    name: 'Joel Mukanya',
                    reference: 'Life Choices Academy Lecturer',
                    image: "https://i.postimg.cc/Px3Mh4GR/Joel-Profile.jpg",
                    message: 'Meezan is very creative, well-behaved, and dedicated; he enjoys working with his Peers and works well on his project. He has learned a variety of skills, such as JavaScript, ExpressJS, MySQL, Wireframe, VueJS, Bootstrap, and many more. I am honored to present him to you as one of the great candidates / developers that you have never come across. I am wishing him all the best.'
                }, 
                {
                    name: 'Brogan Gys',
                    reference: 'Peer',
                    image: "https://i.postimg.cc/Ss0d9Wpj/t2.jpg",
                    message: 'Open, chilled guy who you can easily communicate with. Always willing to help regardless if himself is busy. Does not shy away from a challenge. Understands things quicker than most people.'
                },
                {
                    name: 'Imraan Bernksen',
                    reference: 'Peer',
                    image: "https://i.postimg.cc/T3h9Mgd5/t0.jpg",
                    message: 'Meezaan is a friendly person, he likes to help where he can, always positive and smart with his approach.He is a big football fan and enjoys music. I feel like he will go far in life, whatever he does in the future.'
                },
                {
                    name: 'Cassidy Lawrence',
                    reference: 'Peer',
                    image: "https://i.postimg.cc/TPdz0PZv/Profile.png",
                    message: 'Meezaan is a driven person. He will always make an effort to find a solution and will never hesitate to ask for assistance when necessary. He is a brilliant, intelligent guy who is always willing to give sound advise to anyone who requests it. He also has excellent social skills that make him a wonderful team member. His artistic side nearly never lets him down. He completes tasks once he sets his mind to them.'
                },
                {
                    name: 'Mueen Slamat',
                    reference: 'Peer',
                    image: "https://i.postimg.cc/bv2dkDQB/mueen.jpg",
                    message: 'Meezaan is a chilled and honest guy.He always gives 100% to anything he faces. He will always be willing to help the next person. He is a goal driven individual. A real "COOL" guy.'
                },
                {
                    name: 'Reece Simons',
                    reference: 'Peer',
                    image: "https://i.postimg.cc/R0s5SX6r/reece.jpg",
                    message: 'Meezaan is a very ambitious and always gives best, whilst always being ready to assist others.'
                },
                {
                    name: 'Asandile Langeni',
                    reference: 'Peer',
                    image: "https://i.postimg.cc/kMLxcD7K/Asandile.jpg",
                    message: 'He is a down to earth person, who is always smiling and he is reliable , you can count on him at all time. He is always willing to help people and he does not shy away from showing his soft side. He has a vast awareness of his surroundings and that makes him a focused person.'
                }          
            ]
        }
}
}
</script>

<style scoped>
#testimonials {
    background-image: linear-gradient(white, rgb(103, 172, 224));
    height: auto;
}

.card {
    margin: auto;
    justify-content: center;
    padding: 20px;
    width: 25rem;
    height: 25rem;
    background-color: transparent;
    border-radius: 50%;
    box-shadow: 0 5px 10px rgb(0, 44, 78);
    
}

.card-text, b, h4 {
    font-family: 'Merienda', cursive;
    font-size: 14px;
}

.overlay {
    position: absolute;
    bottom: 0;
    left: 0;
    right: 0;
    color: black;
    background: rgba(255, 255, 255, 0.5);
    backdrop-filter: blur(50px);
    overflow: hidden;
    width: 100%;
    height: 0;
    transition: .5s ease;
  }
  .card:hover .overlay {
    height: 100%;
    border-radius: 50%;
  }

  .text {
     padding: 20px;
  }
.testimonials {
    padding: 100px;
  }
  .testimonials h3 {
    margin-bottom: 20px;
  }
  .testimonials .card {
    border: 3px rgb(0, 44, 78) solid !important;
    transition: 0.5s;
    margin-top: 60px;
  }
  .testimonials .card i {
    background-color: rgb(0, 44, 78);
    color: #ffffff;
    width: 75px;
    height: 75px;
    line-height: 75px;
    margin: -60px auto 0 auto;
  }
  

  


</style>