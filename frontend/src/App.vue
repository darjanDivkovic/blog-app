<template>
<!--
    <nav>
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link>
  </nav> 
-->
  <router-view/>
</template>

<style lang="scss">
html, body {
  margin: 0; 
  padding: 0;
}
#app {
  background-image: linear-gradient(to right, #b7bed0, #b1b8cc, #aab3c8, #a4adc4, #9ea8c0);
  height: 100vh;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  overflow: hidden;
}

nav {

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
