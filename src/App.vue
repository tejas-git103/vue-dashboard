<template>
<div class="app-container">
    <!-- <img alt="Vue logo" src="./assets/logo.png">
  <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  <Menu :selection="selection" @emit-selection="listenSelection" />
  <Home v-if="selection == 'home'"/>
  <Tree v-if="selection == 'tree'"/>
</div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import Home from './components/Home.vue'
import Menu from './components/Menu.vue'
import Tree from './components/Tree.vue'
export default {
  name: 'App',
  data(){
    return{
      selection:'home'
    }
  },
  components: {
    Menu,
    Home,
    Tree
  },
  methods:{
    listenSelection(data){
      this.selection = data;
    }
  }
}
</script>

<style>

.app-container{
  display: flex;
  flex-direction: row;
  
}
/* #app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
} */
</style>
