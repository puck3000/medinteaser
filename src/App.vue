<template>
  <div id="app">
    <Header />
    <main class="animatedColor">
      <router-view />
    </main>
    <!-- <Footer /> -->
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
@font-face 
  font-family: 'SuisseRegular';
  src: url('assets/fonts/SuisseIntl-Regular.otf') format('otf');


html, body 
  margin: 0;
  height: 100vh;
  background-color: rgb(235, 235, 235);


#app 
  margin: 1rem;
  display: flex;
  flex-direction: column;

  h2, a
    font-family: 'SuisseRegular', Helvetica, sans-serif;
    font-weight: 500;
    font-size: 1.5rem
    margin-top: 0
  a 
    color: inherit
    margin-bottom: 0
  
main 
  opacity: 0.6

.animatedColor 
  animation: h2ColorWheel 40s linear infinite;

@media  screen and (min-width: 768px)
  body 
    display: flex;
    justify-content: center;
    align-items: center;
  #app 
    margin: 4rem
    max-width: 1200px
    

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
