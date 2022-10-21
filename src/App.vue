<script setup lang="ts">
import { onBeforeUnmount, onMounted } from 'vue';
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'


const onResize = () => {
  document.documentElement.style.fontSize = window.innerWidth / 1920 * 192 + 'px'

}
onMounted(onResize)
onMounted(() => window.addEventListener('resize', onResize))
onBeforeUnmount(() => window.removeEventListener('resize', onResize))
</script>

<template>
  <!-- <RouterLink to="/">Home</RouterLink>
  <RouterLink to="/about">About</RouterLink> -->
  <!-- <header>
    <img alt="Vue logo" class="logo" src="@/assets/logo.svg" width="125" height="125" />

    <div class="wrapper">
      <HelloWorld msg="You did it!" />

      <nav>
        
      </nav>
    </div>
  </header> -->
  <div class="w-screen h-screen overflow-hidden">
    <RouterView class="w-full h-full" />
  </div>

</template>

<style>
@import './output.css';

</style>
<style scoped>

</style>
