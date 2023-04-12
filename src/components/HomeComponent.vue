<template>
  <div id="home">
    <img class="img-fluid" src="https://i.postimg.cc/SNKr66k3/12345.jpg" alt="">
    <div class="container">
      <h1>Welcome to the Portfolio of <span>Meezaan Davids</span></h1>
      <br />
      <div class="box" style="min-height: 50vh;padding:0"> 
          <ul class="info">
            <li><div class="iam">Aspiring</div></li>
            <li><div class="text"></div></li>
          </ul>
          <ul class="buttons">
            <li><a class="btn" href="#about">Get to Know Me</a></li>
          </ul>
      </div>
    </div>
  </div>
</template>

<script>
import { onMounted } from "vue";
import Typed from "typed.js";

export default {
  setup() {
    let typing = null;

    onMounted(() => {
      typing = new Typed(".text", {
        strings: [
          "Software Developer",
          "Web Developer",
          "FullStack Developer",
          "UX Designer",
        ],
        typeSpeed: 100,
        backSpeed: 40,
        loop: true,
      });
    });

    return {
      typing,
    };
  },
};
</script>

<style scoped>
#home {
  min-height: 100vh;
  position: relative;
}

#home img {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.container {
  position: absolute;
  top: 70%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 100%;
  height: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

h1 {
  text-align: center;
  color: rgb(103, 172, 224);
  font-family: 'Merienda', cursive;
  font-size: 30px;
  z-index: 1;
}

span {
  color: rgb(0, 44, 78);
  font-family: 'Merienda', cursive;
}

.iam {
  color: rgb(103, 172, 224);
  font-size: 25px;
  font-family: 'Merienda', cursive;
}

.text {
  color: rgb(103, 172, 224);
  font-size: 25px;
  font-family: 'Merienda', cursive;
  color: rgb(0, 44, 78);
  text-align: center;
  width: 100%;
  z-index: 1;
}

.info {
  text-align: center;
  width: 100%;
  list-style: none;
  display: flex;
  gap: 20px;
  justify-content: center;
}

.buttons {
  list-style: none;
  display: flex;
  gap: 20px;
  justify-content: center;
}

.btn {
  background: rgb(103, 172, 224);
  color: white;
  border-radius: 3px;
  font-family: 'Merienda', cursive;
  padding: 15px;
}

.btn:hover {
  background: rgb(0, 44, 78);
  color: white;
}
</style>