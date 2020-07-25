<template>
  <div id="app">
    <Header/>
    <router-view/>
    <Footer/>
  </div>
</template>
<script>
import Header from './layouts/Header'
import Footer from './layouts/Footer'

export default {
  components: {
    Header,
    Footer
  }
}
</script>
<style>
@import url('https://fonts.googleapis.com/css?family=Roboto:300,400,500,700|Google+Sans:400,500,700');

#app {
  font-family: 'Roboto', sans-serif;
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
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
