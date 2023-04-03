<template>
  <div id="home">
    <div class="container" style="padding-top: 250px">
      <h1>Welcome to the Portfolio of <span>Meezaan Davids</span></h1>
      <br />
      <div class="box" style="min-height: 50vh;padding:0"> 
          <ul class="info">
            <li><div class="iam">Aspiring</div></li>
            <li><div class="text"></div></li>
          </ul>
          <ul class="buttons">
            <li><a class="btn" href="#">Get to Know Me</a></li>
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
  background: rgb(103, 172, 224);
  height: auto;
}

h1 {
  text-align: center;
  color: white;
  font-family: 'Merienda', cursive;
  font-size: 58px;
}

span {
  color: rgb(0, 44, 78);
  font-family: 'Merienda', cursive;
}
.iam {
  color: white;
  font-size: 45px;
  font-family: 'Merienda', cursive;
}
.text {
  color: white;
  font-size: 45px;
  font-family: 'Merienda', cursive;
  color: rgb(0, 44, 78);
  text-align: center;
  width: 100%;
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
  background: transparent;
  border: 1px solid white;
  color: rgb(0, 44, 78);
  border-radius: 0;
  font-family: 'Merienda', cursive;
  padding: 15px;
}

.btn:hover {
  background: white;
  color: black;
}
</style>
