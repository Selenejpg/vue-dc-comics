<template>
    <ul>
        <li>CHARACTERS</li>
        <li class="active">COMICS</li>
        <li>MOVIES</li>
        <li>TV</li>
        <li>GAMES</li>
        <li>COLLECTIBLES</li>
        <li>VIDEOS</li>
        <li>FANS</li>
        <li>NEWS</li>
        <li>SHOP</li>
    </ul> 
</template>

<script>

export default {
  name: 'NavComp',
}
</script>

<style scoped lang="scss">

@import './style/variabili.scss';

    ul{
        list-style-type: none;
        display: flex;
        align-items: center;
    }

    li{
        margin-right: 25px;
    }

    .active{
        color: $blue;
        border-bottom: 2px solid $blue;
        margin-top: 2px;
        padding: 10px;
    }
</style>