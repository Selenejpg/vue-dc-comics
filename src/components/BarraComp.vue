<template>
      <ul>
          <li>
              <img class="icon" src="/img/buy-comics-digital-comics.png" alt="">
              <span>DIGITAL COMICS</span>
          </li>
          <li>
              <img class="icon" src="/img/buy-comics-merchandise.png" alt="">
              <span>DC MERCHANDISE</span>
          </li>
          <li>
              <img class="icon" src="/img/buy-comics-subscriptions.png" alt="">
              <span>SUBSCRIPTION</span>
          </li>
          <li>
              <img class="icon-locator" src="/img/buy-comics-shop-locator.png" alt="">
              <span>COMIC SHOP LOCATOR</span>
          </li>
          <li class="visa">
              <img class="icon-visa" src="/img/buy-dc-power-visa.svg" alt="">
              <span>DC POWER VISA</span>
          </li>
      </ul>
</template>

<script>

export default {
  name: 'LogoComp',
}
</script>

<style scoped lang="scss">

ul{
    display: flex;
    justify-content: center;
    list-style-type: none;
}

li{
    display: flex;
    justify-content: center;
    align-items: center;
    font-size: 12px;
}

.icon {
    width: 20%;
    margin-right: 15px;
}

.icon-locator{
    width: 12%;
    margin-right: 15px;
}

.icon-visa{
    width: 15%;
    margin-left: -90px;
    margin-right: 15px;
}  

</style>