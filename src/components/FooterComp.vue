<template>
    <footer>
        <div class="col"></div>
        <div class="col padding">
            <h1>DC COMICS</h1>
            <ul class="style-type">
                <li>Characters</li>
                <li>Comics</li>
                <li>Movies</li>
                <li>TV</li>
                <li>Games</li>
                <li>Videos</li>
                <li>News</li>
            </ul>

            <h1  style="margin-top: 15px;">SHOP</h1>
            <ul class="style-type">
                <li>Shop DC</li>
                <li>Shop DC Collectibles</li>
            </ul>

        </div>

        <div class="col padding">
            <h1>DC</h1>
            <ul class="style-type">
                <li>Terms of use</li>
                <li>Privacy policy (New)</li>
                <li>Ad Choices</li>
                <li>Advertising</li>
                <li>Jobs</li>
                <li>Subscriptions</li>
                <li>Talent Workshops</li>
                <li>CPSC Certificates</li>
                <li>Ratings</li>
                <li>Shop Help</li>
                <li>Contact Us</li>
            </ul>
        </div>

        <div class="col padding">
            <h1>SITES</h1>
            <ul class="style-type">
                <li>DC</li>
                <li>MAD Magazine</li>
                <li>DC Kids</li>
                <li>DC Universe</li>
                <li>DC Power visa</li>
            </ul>
        </div>

        <div class="col"></div>
    
        <div class="col mega-logo">
            <img src="/img/dc-logo-bg.png" alt="">
        </div> 

        <div class="col"></div>
      
    </footer>
    
</template>

<script>

export default {
  name: 'FooterComp',
}
</script>

<style scoped lang="scss">
    *{
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      width: 100%;
    }

    footer{
        display: flex;
        width: 100%;
        height: 400px;
        margin: auto;
        background-image: url(/public/img/footer-bg.jpg);
        background-repeat: no-repeat;
        background-size: cover;
        font-size: 13px;
        

        .col {
            width: calc(100%/6);
            color: gray;
        }

        .style-type{
            list-style-type: none;
            text-align: left;
        }

        h1{
            color: white;
            text-align: left;
            font-size: 13px;
        }

        .mega-logo{
          width: 40%;
        }

        .padding{
            padding-top: 6%;
        }
    }
</style>