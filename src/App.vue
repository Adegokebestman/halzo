<template>
  <div id="app">
    <Header/>
      <!-- <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link> -->
    
    <router-view/>
  </div>
</template>


<script>
import Header from './components/layout/Header';
export default {
  name: "app",
  components: {
    Header
  }
}
</script>








<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
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
</style>
