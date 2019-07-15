<template>
  <div class="container">
    <h2>
      Ihr neues Gesundheitszentrum beim Bahnhof Biel.
      <br />ab Oktober 2019
    </h2>
    <div id="dot" class="animatedColor">●</div>
    <h2 class="ta_left">
      Französisches Gesundheitszentrum beim Bahnhof Bienne.
      <br />ab Oktober 2019.
    </h2>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: "home"
};
</script>

<style lang="stylus" scoped>
.container {
  height: 100%;
  font-family: 'SuisseRegular', Helvetica, sans-serif;
  display: flex;
  flex-direction: column;
  justify-content: center;
}

h2 {
  &.ta_left {
    text-align: right
  }
}

#dot {
  line-height: 9rem;
  font-size: 15rem;
  text-align: center;
  opacity: 0.7
  margin-bottom: 1.5rem
}
</style>
