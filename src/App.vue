<template>
  <div id="nav">
    <a style="font-size: 24px;">Home Page Site</a>
    <router-link to="/">Top</router-link>
    <router-link to="/home">Home</router-link>
    <router-link to="/about">About</router-link>
    <router-link to="/contact">Contact</router-link>
  </div>
  <router-view/>
  <p class="copyright">
    &copy; {{ now }} Home Page Site.
  </p>
</template>

<script>
export default {
  data: () => {
    return {
      now: ''
    };
  },
  created () {
    const d = new Date()
    this.now = d.getFullYear()
  }
}
</script>

<style>
body {
  background-image: url("./assets/background.jpg");
  background-repeat: repeat;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
  background-color: beige;
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
