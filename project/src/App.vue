<template>
  <div id="app">
    <NavBar></NavBar>
    <SideBar></SideBar>
    <Player></Player>
  </div>
</template>

<script>
import SideBar from '@/components/SideBar.vue'
import NavBar from '@/components/NavBar.vue'
import Player from '@/components/Player.vue'

export default {
  name: 'App',
  components: {
    SideBar,
    NavBar,
    Player
  }
}
</script>

<style>
#app{
 
}
body{
  background:#2d3748;
  background-size: cover;
}
</style>
