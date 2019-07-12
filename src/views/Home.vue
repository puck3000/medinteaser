<template>
  <div id="container">
    <Logo/>
  </div>
</template>

<script>
// @ is an alias to /src
import Logo from '@/components/Logo.vue'

export default {
  name: 'home',
  components: {
    Logo
  }
}
</script>

<style lang="stylus" scoped>
#container 
  width: 100%
  height: 100%
  display: grid
  justify-items: center 
  align-items: center

</style>
