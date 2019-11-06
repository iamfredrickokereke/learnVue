<template>
  <div id="app">
    <h1>Hello, {{msg}}  </h1>
    <Navbar />
    <Container />
  </div>
</template>

<script>
import Navbars from './Navbar';
import Container from './Container'

export default {
  name: 'app',
  components: {
    Navbar:Navbars,
    Container:Container

  },
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
