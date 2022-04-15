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
    ul{
        list-style-type: none;
        display: flex;
        align-items: center;
    }

    li{
        margin-right: 25px;
    }

    .active{
        color: #0282f9;
        border-bottom: 2px solid #0282f9;
        margin-top: 2px;
        padding: 10px;
    }
</style>