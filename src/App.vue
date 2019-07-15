<template>
  <div id="app">
    <Header />
    <main>
      <router-view />
    </main>
    <Footer />
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import Footer from "@/components/Footer.vue";

export default {
  name: "app",
  components: {
    Header,
    Footer
  }
};
</script>

<style lang="stylus">
@font-face {
  font-family: 'SuisseRegular';
  src: url('assets/fonts/SuisseIntl-Regular.otf') format('otf');
}

html, body {
  margin: 0;
  height: 100vh;
  background-color: rgb(235, 235, 235);
}

#app {
  height: calc(100% - 2rem)
  margin: 1rem;
  display: flex;
  flex-direction: column;

  h2 {
    font-family: 'SuisseRegular', Helvetica, sans-serif;
    font-weight: 500;
    margin: 0
  }
}

main {
  flex: 1;
}

.animatedColor {
  animation: h2ColorWheel 40s linear infinite;
}


@media  screen and (min-width: 768px)
  body 
    display: flex;
    justify-content: center;
    align-items: center;
  #app 
    margin: 4rem
    height: calc(100% - 8rem)
    max-width: 768px
    


@keyframes h2ColorWheel {
  0% {
    color: rgb(105, 105, 105); // darkGrey
  }

  14% {
    color: rgb(105, 105, 105); // darkGrey
  }

  16% {
    color: rgb(167, 0, 0); // darkRed
  }

  29% {
    color: rgb(167, 0, 0); // darkRed
  }

  31% {
    color: rgb(175, 91, 0); // darkOrange
  }

  44% {
    color: rgb(175, 91, 0); // darkOrange
  }

  46% {
    color: rgb(0, 0, 183); // darkBlue
  }

  59% {
    color: rgb(0, 0, 183); // darkBlue
  }

  61% {
    color: rgb(4, 151, 92); // darkGreen
  }

  74% {
    color: rgb(4, 151, 92); // darkGreen
  }

  76% {
    color: rgb(250, 0, 255); // darkMagenta
  }

  99% {
    color: rgb(250, 0, 255); // darkMagenta
  }

  100% {
    color: rgb(105, 105, 105); // darkGrey
  }
}
</style>
