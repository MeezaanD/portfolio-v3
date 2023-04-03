<template>
    <div id="contact">
        <h6 class="heading">Contact</h6>
        <div class="container">
            <div class="content">
              <div data-aos="zoom-out-right" class="left-side">
                <div class="address details">
                  <i class="fas fa-map-marker-alt"></i>
                  <div class="topic">Address</div>
                  <div class="text-one">Grassy Park, Cape Town, Western Cape</div>
                </div>
                <div class="phone details">
                  <i class="fas fa-phone-alt"></i>
                  <div class="topic">Cell</div>
                  <div class="text-one">0658707217</div>
                </div>
                <div class="email details">
                  <i class="fas fa-envelope"></i>
                  <div class="topic">Email</div>
                  <div class="text-one">meezaandavids365@gmail.com</div>
                </div>
                <ul>
                    <li><a href="https://www.instagram.com/meezaan.davids/" target="_blank"><i class="fa-brands fa-instagram"></i></a></li>
                    <li><a href="https://github.com/MeezaanD" target="_blank"><i class="fa-brands fa-github"></i></a></li>
                    <li><a href="https://www.linkedin.com/in/meezaan-davids-4a7aa8265/" target="_blank"><i class="fa-brands fa-linkedin"></i></a></li>
                </ul>
              </div>
              <div data-aos="zoom-out-down" class="right-side">
                <div class="topic-text">Send me a message</div>
                <p>Thank you for reviewing my portfolio, if there is anything else you wish to know do not hesitate to contact me</p>
              <form action="https://formspree.io/f/mbjbywlp" method="post">
                <div class="input-box">
                  <input type="text" placeholder="Enter your name" name="name" required>
                </div>
                <div class="input-box">
                  <input type="number" placeholder="Enter your cell" name="number" required>
                </div>
                <div class="input-box">
                  <input type="email" placeholder="Enter your email" name="email" required>
                </div>
                <div class="button">
                  <input type="submit" value="Reach Me">
                </div>
              </form>
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
#contact {
    background-image: linear-gradient(rgb(103, 172, 224), white);
    min-height: 90vh;
}

ul {
    list-style: none;
    display: flex;
    gap: 40px
}

.fa-instagram,
.fa-github,
.fa-linkedin,
.fa-twitter {
  color: rgb(0, 44, 78);
  font-size: 30px;
  padding-top: 50px;
}
.container{
  display: flex;
  background: transparent;
  justify-content: center;
  border-radius: 6px;
  padding: 60px;
  box-shadow: 0 5px 10px rgb(0, 44, 78);
}
.container .content{
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.container .content .left-side{
  width: 25%;
  height: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  margin-top: 15px;
  position: relative;
}
.content .left-side::before{
  content: '';
  position: absolute;
  height: 70%;
  width: 2px;
  right: -15px;
  top: 50%;
  transform: translateY(-50%);
  background: transparent;
}
.content .left-side .details{
  margin: 14px;
  text-align: center;
}
.content .left-side .details i{
  font-size: 30px;
  color: rgb(0, 44, 78);
  margin-bottom: 10px;
}
.content .left-side .details .topic{
  font-size: 18px;
  font-weight: 500;
}
.content .left-side .details .text-one{
  font-size: 15px;
  font-family: 'Merienda', cursive;
  font-weight: 800;
  color: white;
  -webkit-text-stroke: 1px rgb(0, 44, 78);
}
.container .content .right-side{
  width: 75%;
  margin-left: 75px;
}
.content .right-side .topic-text{
  font-size: 23px;
  font-weight: 600;
  font-family: 'Merienda', cursive;
  color: rgb(0, 44, 78);
}
.right-side .input-box{
  height: 50px;
  width: 100%;
  margin: 12px 0;
}
.right-side .input-box input{
  height: 100%;
  width: 100%;
  border: 1px solid white;
  font-size: 16px;
  color: white;
  background: transparent;
  border-radius: 1px;
  padding: 0 15px;
  resize: none;
}
.right-side .message-box{
  min-height: 110px;
}
.right-side .input-box textarea{
  padding-top: 6px;
}
.right-side .button{
  display: inline-block;
  padding-top: 150px;
  margin-top: 12px;
}
.right-side .button input[type="submit"]{
  color: white;
  font-family: 'Merienda', cursive;
  font-size: 18px;
  border: 3px solid white;
  padding: 8px 16px;
  border-radius: 6px;
  background: rgb(0, 44, 78);
  cursor: pointer;
  transition: all 0.3s ease;
}
.button input[type="submit"]:hover{
  background: rgb(0, 44, 78);
}

@media (max-width: 950px) {
  .container{
    width: 90%;
    padding: 30px 40px 40px 35px ;
  }
  .container .content .right-side{
   width: 75%;
   margin-left: 55px;
}
}
@media (max-width: 820px) {
  .container{
    margin: 40px 0;
    height: 100%;
  }
  .container .content{
    flex-direction: column-reverse;
  }
 .container .content .left-side{
   width: 100%;
   flex-direction: row;
   margin-top: 40px;
   justify-content: center;
   flex-wrap: wrap;
 }
 .container .content .left-side::before{
   display: none;
 }
 .container .content .right-side{
   width: 100%;
   margin-left: 0;
 }
}




</style>