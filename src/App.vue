<template>
  <head>
    <link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@100..900&display=swap" rel="stylesheet">
  </head>
  <div id="app">
    <Navbar />
    <Home />
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue'
import Home from './components/Home.vue'

export default {
  name: 'App',
  components: {
    Navbar,
    Home
  }
}
</script>

<style>
body {
  margin: 0;
  font-family: Arial, sans-serif;
}
</style>
