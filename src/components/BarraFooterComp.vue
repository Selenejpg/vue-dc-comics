<template>
   <div class="flex">
       <div class="button flex-li"><h2>SIGN-UP NOW!</h2></div>
       <div class="flex-li font-size">
           <h1>FOLLOW US</h1>
           <ul>
               <li><img src="/img/footer-facebook.png" alt=""></li>
               <li><img src="/img/footer-twitter.png" alt=""></li>
               <li><img src="/img/footer-youtube.png" alt=""></li>
               <li><img src="/img/footer-pinterest.png" alt=""></li>
               <li><img src="/img/footer-periscope.png" alt=""></li>
           </ul>
       </div>
   </div>
</template>

<script>

export default {
  name: 'BarraFooterComp',
}
</script>

<style scoped lang="scss">

@import './style/variabili.scss';

*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    width: 100%;
    background-color: #303030;
    color: white;
}

.flex{
    display: flex;
    justify-content: space-evenly;
    padding-left: 20%;
    padding-top: 40px;
    padding-bottom: 40px;
}

ul{
    list-style-type: none;
    display: flex;
}

li{
    width: 6%;
    margin-right: 10px;
}

.flex-li{
    display: flex;
    align-items: center;
}

.font-size{
    font-size: 10px;
}

h1{
    width: 40%;
    margin-left: 45%;
}

.button {
    border: 1px solid $blue;
    width: 14%;
    font-size: 10px;
    text-align: center;
    padding: 10px;
}

</style>