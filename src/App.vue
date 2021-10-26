<template>
  <transition name="router-anim">
    <router-view />
  </transition>
</template>

<script>
export default {
  name: "App",
};
</script>

<style scoped>
  #app{
    position: relative;
  }
</style>