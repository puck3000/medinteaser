<template>
  <div id="app">
    <header></header>
  <main> 
    <router-view/>
  </main>
  <footer></footer>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="stylus">
  html, body, #app, main 
    margin: 0
    height: 100vh
    font-family: "Futura Std", "sans-serif"
</style>
