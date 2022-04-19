<template>
  <div class="main-active product">
    <div class="box">
      <img :src="details.src" alt="">
      <h3>{{ details.titolo }}</h3>
    </div>
  </div>

</template>

<script>

export default {
  name: 'ProductComp',
  props: ['details']
}
</script>

<style scoped lang="scss">

@import './style/variabili.scss';

  *{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }

  .main-active {
    background-color: black;
    color: white;
    text-align: center;
    padding: 30px;
  }

.product {
  display: flex;
  flex-basis: calc(100% / 6);

  img {
    width: 100%;
  }

  h3 {
    font-size: 12px;
  }
}


</style>