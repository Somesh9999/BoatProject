<template>
  <router-view/>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600;800&display=swap');
body{
  font-size: 15px;
  font-family: 'Poppins', sans-serif;
  /* font-family: "Fogie"; */
  margin: 0;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  /* color: #2c3e50; */
  color: white;
  text-decoration: none;
}

nav a.router-link-exact-active {
  /* color: #42b983; */
  color: white;
}

@font-face {
  font-family: "Fogie";
  src: local("Fogie"),
   url(./fonts/fogie/Fogie-Regular.ttf) format("truetype");
}
</style>
