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
  font-family: 'Futura Std'
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
    line-height: 1.5
    font-weight: 450;
  .dot 
    position: absolute
    left: 13.7rem
    height: 1.5rem
    -webkit-filter: blur(0);
    transition: transform 1s ease-in-out 1s
    transform: scale(1) 
    &:hover 
      transform: scale(50)

    circle 
      fill: red
      cx: 60
      cy: 60
      r: 50
  h2 
    margin: 0
    font-size: 2.5rem
    font-weight: 50


</style>
