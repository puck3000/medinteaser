<template>
  <div id="app" :style="{color: currentColor}">
    <Head :color="currentColor" />
    <main class="animatedColor">
      <router-view />
    </main>
  </div>
</template>

<script>
import Head from "@/components/Head.vue";

export default {
  name: "app",
  components: {
    Head
  },
  data() {
    return {
      colors: ["#0000ff", "#ff0900", "#ffa200", "#49e6a3", "#ff00ff"],
      currentColor: "#0000ff",
      i: 0
    };
  },
  methods: {
    nextColor: function() {
      let self = this;
      setInterval(function() {
        self.i = (self.i + 1) % 5;
        self.currentColor = self.colors[self.i];
      }, 10000);
    }
  },
  beforeMount() {
    this.nextColor();
  }
};
</script>

<style lang="stylus">
// --------------------------------------
// VARS
// -------------------------------------
:root {
  --theme_blue: #0000ff;
  --theme_red: #ff0900;
  --theme_orange: #ffa200;
  --theme_green: #49e6a3;
  --theme_pink: #ff00ff;
}

// --------------------------------------
// FONTS
// -------------------------------------
@font-face {
  font-family: 'SuisseRegular';
  src: url('assets/fonts/SuisseIntl-Regular.otf') format('otf');
}

html, body {
  margin: 0;
  height: 100vh;
  // background-color: rgb(235, 235, 235);
}

h1, h2, a {
  font-family: 'SuisseRegular', Helvetica, sans-serif;
  font-weight: 500;
  font-size: 1.5em;
  margin-top: 0;
  color: inherit;
}

// --------------------------------------
// GENERAL LAYOUT
// -------------------------------------
#app {
  margin: 1rem;
  transition: color 2s ease-in-out;
}

@media screen and (min-width: 768px) {
  body {
    display: flex;
    justify-content: center;
    align-items: center;
  }

  #app {
    margin: 4rem;
    max-width: 1200px;
  }
}
</style>
