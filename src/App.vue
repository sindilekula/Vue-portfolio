<template>
  <Navbar />
  <!-- <nav>
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link> |
    <router-link to="/contact">Contact</router-link> |
    <router-link to="/projects">Projects</router-link> |
    <router-link to="/resume">Resume</router-link> |
    <router-link to="/testimonials">Testimonials</router-link>
  </nav> -->
  <router-view/>
  <Footer />
</template>

<script>
// import Landing from "./components/Landing.vue";
import Navbar from "./components/Navbar.vue";
import Footer from "./components/Footer.vue";


export default {
  name: "App",
  components: {
    Navbar,
    Footer,
  },
};
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap');

#app {
  font-family: Cormorant SC;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  overflow-x: hidden;
  /* color: #2c3e50; */
  
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}


</style>
