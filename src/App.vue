<template>
  <div id="nav">
    <div v-for="(route, index) in router.options.routes" :key="route.name" class="nav-item">
      <router-link :to="route.path">{{ route.name }}</router-link> <span v-if="index != router.options.routes.length-1">| </span>
    </div>
  </div>
  <router-view/>
</template>
<script lang="ts">
import router from '@/router/index'

export default {
  name: 'App',
  data(){
    return{
      router
    }
  }
}
</script>
<style >
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
a{
  text-decoration: none;
}
.container{
  margin-top: 50px;
}
#nav {
  position: fixed;
   left: 0;
   bottom: 10px;
   width: 100%;
   text-align: center;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
  text-decoration: none;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
.nav-item{
  display:inline;
  
}
</style>