<template>
  <div id="app" class="app-box">
    <Search />
    <Show />
    <Favorit />
  </div>
</template>

<script>
import Show from "./components/Show.vue";
import Search from "./components/Search.vue";
import Favorit from './components/Favorit.vue'
/**
 * search组件
 * show组件
 */
export default {
  components: {
    Show,
    Search,
    Favorit,
  },
};
</script>



<style>
.app-box {
  display: flex;
  flex-direction: column;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
 
  color: #2c3e50;
  margin: 50px 0 0 50px;
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
