<template>
   <header class="header">
       <h1>Halzo</h1>
        <router-link to="/">Home</router-link> |
      <router-link to="/about">Todo</router-link>
   </header>   
</template>


<script>
export default {
  name: "Header"  
}
</script>

<style scoped>
.header{
    background: #E44232;
    color: #ffffff;
    text-align: center;
    padding: 10px;
}
.header a{
    color: #ffffff;
    padding-right: 5px;
    text-decoration: none;
}
a:hover{
    color: #42b983;
}
</style>