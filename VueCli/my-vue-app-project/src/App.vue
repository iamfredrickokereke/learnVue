<template>
  <div id="app">
    <h1>Hello, {{msg}}  </h1>
    <Navbars />
    <myContainers />
    <Friends :friends="friends" @delete="deleteFriend"/>
    <Online :friends="friends"/>
    
  </div>
</template>

<script>
import Navbars from './Navbar'
import myContainers from './Container'
import Friends from './Friends'
import Online from './Online'


export default {
  name: 'app',
  components: {
    Navbars,
    myContainers,
    Friends,
    Online 
  },
  data () {
    return {
      msg: 'Welcome to My Vue.js App',
      friends:[
                     
                    {name : 'fred', status : true},
                    {name : 'emma', status : true},
                    {name : 'charles', status : false},
                    {name : 'nonso', status : false}
      ]      
    }
  },
  methods:{
    deleteFriend(payload){
      this.friends = this.friends.filter(friend => {
        return friend.name !== payload.name
      })
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
