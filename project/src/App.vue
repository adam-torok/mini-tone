<template>
  <div id="app">
    <transition
        mode="out-in"  
        enter-active-class="animated fadeIn"
        leave-active-class="animated fadeOut">
      <router-view>
      </router-view>
    </transition>
  </div>
</template>

<script>
export default {
  name: 'App',
}
</script>

<style>
body{
  background:#2d3748;
  background-size: cover;
}
</style>
