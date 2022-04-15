<template>
  <div id="app">
    <header>
      <LogoComp/>
      <NavComp/>
    </header>
    <main>
      <div class="main-active"><h2>Il contenuto va qui</h2></div>
      <div class="main-barra"><BarraComp/></div>
    </main>
    <footer>
      <FooterComp/>
    </footer>
  </div>
</template>

<script>
import LogoComp from './components/LogoComp.vue'
import NavComp from './components/NavComp.vue'
import BarraComp from './components/BarraComp.vue'
import FooterComp from './components/FooterComp.vue'

export default {
  name: 'App',
  components: {
    LogoComp,
    NavComp,
    BarraComp,
    FooterComp
  }
  
}
</script>

<style lang="scss">

@import './components/style/variabili.scss';

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  display: flex;
  flex-wrap: wrap;
}

*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

header {
  width: 100%;
  display: flex;
  justify-content: space-evenly;
  padding: 20px;
}

main {
    width: 100%;
}

.main-active {
  background-color: black;
  color: white;
  text-align: center;
  padding: 40px;
}

.main-barra{
  background-color: $blue;
  color: white;
  padding: 50px;
}
</style>
