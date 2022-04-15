<template>
  <div id="app">
    <header>
      <LogoComp/>
      <NavComp/>
    </header>
  </div>
</template>

<script>
import LogoComp from './components/LogoComp.vue'
import NavComp from './components/NavComp.vue'

export default {
  name: 'App',
  components: {
    LogoComp,
    NavComp
  }
  
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  display: flex;
  flex-wrap: wrap;
}

header {
  width: 100%;
  display: flex;
  justify-content: space-evenly;
  padding: 10px;
}
</style>
