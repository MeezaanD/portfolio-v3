<template>
  <NavBar/>
  <!-- <nav>
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link>
  </nav> -->
  <router-view/>
</template>

<script>

import NavBar from '@/components/NavBar.vue'

export default {
  components: { NavBar}
}
</script>


<style>
@import url('https://fonts.googleapis.com/css2?family=Merienda&display=swap');


@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@200;300;400;500;600;700&display=swap');

**{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  scroll-behavior: smooth;
}

h6 {
  text-align: center;
  padding: 30px;
  font-family: 'Merienda', cursive;
}

h6::after {
  content: "";
  display: block;
  width: 5%;
  margin: 0 auto;
  border-bottom: 2px solid black;
  margin-top: 10px;
}

::-webkit-scrollbar {
  width: 20px;
}

::-webkit-scrollbar-track {
  border-radius: 50%;
  background: transparent;
}

::-webkit-scrollbar-thumb {
  border-radius: 50%;
  background-image: linear-gradient(rgb(103, 172, 224), white, rgb(103, 172, 224));
}
</style>
