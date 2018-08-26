<template>
  <Home></Home>
</template>

<script>
import Home from './components/Home.vue'

export default {
  name: 'app',
  components: {
    Home
  }
}
</script>

<style>
@import "tailwindcss/preflight";
@import "tailwindcss/components";
@import "tailwindcss/utilities";
</style>
