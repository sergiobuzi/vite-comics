<script>
    export default{
        name:"AppFooter",
        data() {
            return {
            
            }
        }
    }
</script>

<template>
    <div id="container">
        <div id="box-ul">
            <div id="box-ul-left">
                <ul>DC COMICS
                    <li>Characters</li>
                    <li>Comics</li>
                    <li>Movies</li>
                    <li>TV</li>
                    <li>Games</li>
                    <li>Video</li>
                    <li>News</li>
                </ul>
                <ul>SHOP
                    <li>Shop DC</li>
                    <li>Shop DC Collectables</li>
                </ul>
            </div>

            <div id="box-ul-middle">
                <ul>DC
                    <li>Terms of Use</li>
                    <li>Privacy policy (New)</li>
                    <li>Ad Choices</li>
                    <li>Advertising</li>
                    <li>Jobs</li>
                    <li>Subscription</li>
                    <li>Talent workshop</li>
                    <li>CPSC Certificates</li>
                    <li>Ratings</li>
                    <li>Shop Help</li>
                    <li>Contact Us</li>
                </ul>
            </div>

            <div id="box-ul-right">
                <ul>SITES
                    <li>DC</li>
                    <li>MAD Magazine</li>
                    <li>DC Kids</li>
                    <li>DC Universe</li>
                    <li>DC Power Visa</li>
                </ul>
            </div>
        </div>


        <div id="img-container"></div>

    </div>

    <div id="social-section">

        <div>
            <a id="button">SIGN-UP NOW!</a>
        </div>

        <div>
            <div id="socials"> 
                <h3>FOLLOW US</h3>
                <img src="../assets/img/footer-facebook.png" alt="">
                <img src="../assets/img/footer-twitter.png" alt="">
                <img src="../assets/img/footer-youtube.png" alt="">
                <img src="../assets/img/footer-pinterest.png" alt="">
                <img src="../assets/img/footer-periscope.png" alt="">
            </div>
        </div>
    </div>


</template>

<style lang="scss" scoped>
@use '../styles/general.scss' as *;
@use '../styles/partials/variables' as *;


// parte superiore

#container{
    background-image:url(../assets/img/footer-bg.jpg) ;
    background-size: cover;
    background-repeat: no-repeat;
    width: 100%;
    height: 350px;
    display: flex;
    justify-content: space-around;
    align-items: center;
    

    ul{
        font-weight: 600;
        margin-right: 20px;
        margin-bottom: 10px;
        

        li{
            color: grey;
            font-weight: 100;
            list-style-type: none;
            padding-bottom: 5px;
            font-size: 15px;
        }

        li:hover,
        li:active{
            color: white;
            cursor: pointer;
        }
    }
}

#box-ul{
 display: flex;
}

#img-container{
    background-image: url(../assets/img/dc-logo-bg.png);
    height: 100%;
    width: 40%;
    background-position: center;
    background-repeat: no-repeat;
}



// parte inferiore con i social

#social-section{
    background-color: #313031;
    height: 110px;
    width: 100%;
    display: flex;
    justify-content: space-around;
    align-items: center;
}

#button{
    padding: 10px;
    border: 2px $primary solid;
    cursor: pointer;
}

#socials{
    color: $primary;
    display: flex;
    align-items: center;
    gap: 15px;
    font-weight: 400;
}

</style>