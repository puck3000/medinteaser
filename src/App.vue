<template>
  <main>
    <section>
      <svg class="dot" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 120 120" version="1.1">
        <circle />
      </svg>
      
      <h1>MEDIN</h1>
      <h2>Biel / Bienne</h2>
    </section>
  </main>
</template>
<style lang="stylus">
html, body, main
  width: 100%
  height: 100%
  margin: 0
  padding: 0
  font-family: 'Jost'
main 
  position: relative
section
  position: absolute
  top: 50%
  left: 50%
  transform: translate(-50%, -50%)
  // background-color pink
  // background-clip: text
  // color: transparent
  h1
    color: black
    font-size: 6rem
    margin: 0
    line-height: 1
  .dot 
    position: absolute
    left: 13.55rem
    top: -2rem
    height: 1.5rem
    circle 
      fill: red
      cx: 60
      cy: 60
      r: 50
  h2 
    margin: 0
    font-size: 2.5rem
    font-weight: 400


</style>
