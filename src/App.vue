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
html, body, #app {
  margin: 0;
  height: 100vh;
  background-color: rgb(235, 235, 235);
}

#app {
  margin: 1rem;
  display: flex;
  flex-direction: column;
}

main {
  flex: 1;
}
</style>
