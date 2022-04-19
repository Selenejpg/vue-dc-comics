<template>
  <div id="app">
    <header>
      <LogoComp/>
      <NavComp/>
    </header>
    <div class="container">
      <img class="jumbo" src="../public/img/jumbotron.jpg" alt="">
    </div>
    <main>
      <div class="margin">
        <div class="current">
          <h1>CURRENT SERIES</h1>
        </div> 
      </div>

      <div class="products">
        <ProductComp 
          v-for="(element, index) in products" 
          :key="index"
          :details="element"
        />
      </div>
      <div class="flex">
        <div class="button">
          <h1>LOAD MORE</h1>
        </div> 
      </div>
          
      <div class="main-barra"><BarraComp/></div> 
    </main>
    
    <FooterComp/>  
    <BarraFooterComp/>   
  </div>
</template>

<script>
import LogoComp from './components/LogoComp.vue'
import NavComp from './components/NavComp.vue'
import BarraComp from './components/BarraComp.vue'
import FooterComp from './components/FooterComp.vue'
import BarraFooterComp from './components/BarraFooterComp.vue'
import ProductComp from './components/ProductComp.vue'

export default {
  name: 'App',
  components: {
    LogoComp,
    NavComp,
    BarraComp,
    FooterComp,
    BarraFooterComp,
    ProductComp
  },
  data() {
    return{
      products: [
        {
          src: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
          titolo: "Action Comics", 
        },
        {
          src: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
          titolo: "American Vampire 1976", 
        }, 
        {
          src: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
          titolo: "Aquaman", 
        },
        {
          src: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
          titolo: "Batgirl", 
        },
        {
          src: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          titolo: "Batman", 
        },
        {
          src: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          titolo: "Batman Beyond", 
        }, 
        {
          src: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
          titolo: "Batman/Superman", 
        },
        {
          src: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
          titolo: "Batman/Superman Annual", 
        },
        {
          src: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
          titolo: "Batman: The Joker War Zone", 
        },
        {
          src: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
          titolo: "Batman: Three Jokers", 
        }, 
        {
          src: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
          titolo: "Batman: White Knight Presents: Harley Quinn", 
        },
        {
          src: "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
          titolo: "Catwoman", 
        }
      ]
    }
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
  background-color: black;
}

h1 {
  font-size: 12px;
}

.products{
  width: 80%;
  margin: 0 auto;
  display: flex;
  flex-wrap: wrap;
  padding: 10px;
}

.main-barra{
  background-color: $blue;
  color: white;
  padding: 50px;
}

.button{
  width: 10%;
  color: white;
  background-color: $blue;
  padding: 10px;
}

.flex{
  display: flex;
  justify-content: center;
  padding-bottom: 30px;
}

.margin {
  margin-left: 185px;
  padding-top: 30px;
}

.current {
  width: 10%;
  color: white;
  background-color: $blue;
  padding: 10px;
}

.jumbo {
  max-width: 100vw;
}

.container {
  height: 60vh;
}
</style>
