<template>
  <div id="nav">
    <router-link style="font-size: 24px;" to="/">BinSite</router-link>
    <router-link to="/home">自己紹介</router-link>
    <router-link to="/about">事業内容</router-link>
    <router-link to="/contact">お問い合わせ</router-link>
  </div>
  <br>
  <router-view/>
  <br>
  <br>
  <div id="footer">
    <p class="copyright">
      &copy; {{ now }} BinSite.
    </p>
  </div>
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

#footer {
  padding: 5px;
  background-color: beige;
}

#footer p {
  font-weight: lighter;
  color: #2c3e50;
  margin-left: 30px;
  margin-right: 30px;
}
</style>
