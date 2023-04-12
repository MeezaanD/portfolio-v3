<template>
    <footer>
        <div class="container text-center">
            <div class="row align-items-center">
                <!-- <div class="col-sm-4">
                    <a href="#"><img src="https://i.postimg.cc/g224F76q/logo.png" style="height:7vh" alt=""></a>
                </div>
                <div class="col-sm-4 text-center">
                  <a href="#home">Home</a><br>
                  <a href="#about">About</a><br>
                  <a href="#resume">Resume</a><br>
                  <a href="#projects">Projects</a><br>
                  <a href="#testimonials">Testimonials</a><br>
                  <a href="#contact">Contact</a><br>
                </div>
              <div class="col-sm-4 text-center">
                <p>&copy;Copyright {{ thisYear }} | Designed By Meezaan Davids</p>
              </div> -->
              <p>&copy;Copyright {{ thisYear }} | Designed By Meezaan Davids</p>
            </div>
          </div>
    </footer>
</template>
<script>
export default {
    data(){
	return {
		thisYear : new Date().getFullYear()
	}
  }
}
</script>
<style scoped>
    footer {
        height: auto;
        padding: 30px;
        background: rgba(202,202,202,255);
    }

    a {
        text-decoration: none;
        font-family: 'Merienda', cursive;
        font-size: 14px;
        color: rgb(0, 44, 78);
        font-weight: 700;
    }

    p {
        font-family: 'Merienda', cursive;
        font-size: 14px;
        color: rgb(0, 44, 78);
        font-weight: 700;
    }
</style>