<template>
  <div id="nav">
    <a>Home Page Site</a>
    <router-link to="/">Top</router-link>
    <router-link to="/home">Home</router-link>
    <router-link to="/about">About</router-link>
  </div>
  <router-view/>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
  margin-left: 30px;
  margin-right: 30px;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
