<template>
  <div id="app">
    <Navbar></Navbar>
    <router-view/>
    <Footer></Footer>
  </div>
</template>

<script>
// @ is an alias to /src
import Navbar from '@/components/Navbar'
import Footer from '@/components/Footer';

export default {
  name: 'app',
  components: {
    Navbar,
    Footer
  },
  data () {
    return {
      data: []
    }
  },
}
</script>

<style>
  body {
  background-color: black;
  background-attachment: fixed;
  }

  #app {
    font-family: "Avenir", Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: white;
  }
  
  #nav {
    padding: 30px;
  }
  
  #nav a {
    font-weight: bold;
    color: #2c3e50;
  }
  
  #nav a.router-link-exact-active {
    color: #42b983;
  }

  #inspire {
      height: 100vh 
  }
</style>
