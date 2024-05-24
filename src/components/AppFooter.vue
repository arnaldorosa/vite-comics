<script>
    export default {
        name: "AppFooter",

        data() {
            return { 
                comicsLIst: [
                    "CHARACTERS",
                    "COMICS",
                    "MOVIES",
                    "TV",
                    "Games",
                    "Videos",
                    "News"
                ],
                shopList: [
                    "Shop DC",
                    "Shop DC Collectibles"
                ],
                dcList: [
                    "Terms Of Use",
                    "Privacy Policy (New)",
                    "Ad Choices",
                    "Advertising",
                    "Jobs",
                    "Subscriptions",
                    "Talent Workshop",
                    "CPSC Certificates",
                    "Rating",
                    "Shop Help",
                    "Contact Us"
                ],
                siteList: [
                    "DC",
                    "MAD Magazine",
                    "DC Kids",
                    "DC Universe",
                    "DC Power Visa"
                ],
                iconeSocial: [
                "../src/assets/img/footer-facebook.png",
                "../src/assets/img/footer-twitter.png",
                "../src/assets/img/footer-youtube.png",
                "../src/assets/img/footer-pinterest.png",
                "../src/assets/img/footer-periscope.png"
                ],
                blueBarIcons: [
                    {
                        img: "../src/assets/img/buy-comics-digital-comics.png",
                        text: "DIGITAL COMICS"
                    },
                    {
                        img: "../src/assets/img/buy-comics-merchandise.png",
                        text: "DC MERCHANDISE"
                    },
                    {
                        img: "../src/assets/img/buy-comics-subscriptions.png",
                        text: "SUBSCRIPTION"
                    },
                    {
                        img: "../src/assets/img/buy-comics-shop-locator.png",
                        text: "COMIC SHOP LOCATOR"
                    },
                    {
                        img: "../src/assets/img/buy-dc-power-visa.svg",
                        text: "DC POWER VISA"
                    }
                ]
            }
        }  
    }
</script>

<template>
    <footer>
        <section class="s1">
            <div class="blueBar">
                <div v-for="icone in blueBarIcons" :key="icone">
                    <img :src="icone.img" alt=""  width="50" height="50">
                    <span>{{ icone.text }}</span>
                </div>
            </div>
        </section>
        <section class="s2">
            <div class="footerList">
                <ul>
                    <h3>DC COMICS</h3>
                    <li v-for="comic in comicsLIst">
                        {{comic }}
                    </li>
                </ul>
                <ul>
                    <h3>SHOP</h3>
                    <li v-for="shop in shopList">
                        {{shop}}
                    </li>
                </ul>
                <ul>
                    <h3>DC</h3>
                    <li v-for="dc in dcList">
                        {{dc}}
                    </li>
                </ul>
                <ul>
                    <h3>SITES</h3>
                    <li v-for="site in siteList">
                        {{site}}
                    </li>
                </ul>
            </div>
            <div class="imgContainer">
                <div class="transpBg"></div>
            </div>
        </section>
        <section class="s3">
            <div class="containerS3">
                <div>
                    <button class="signUp">SIGN-UP NOW!</button>
                </div>
                <div>
                    <span class="followUs">FOLLOW US</span>
                    <img class="icone" v-for="icone in iconeSocial" :src="icone">
                </div>
            </div>
        </section>
    </footer>
</template>

<style>
    .s1 {
        background-color: #0282f9;
        width: 100%;
        height: 10rem;
    }

    .s2 {
        display: flex;
        background-image: url(../assets/img/footer-bg.jpg);
        background-repeat: no-repeat;
        background-size: cover;
        width: 100%;
        height: 27.2rem;
    }

    .s3 {
        background-color: #303030;
        width: 100%;
        height: 10rem;
    }

    .imgContainer {
        width: 50%;
        height: 25rem;
        overflow: hidden;
    }
    
    .transpBg {
        width: 70%;
        height: 500px;
        background-image: url(../assets/img/dc-logo-bg.png);
        background-repeat: no-repeat;
        background-size: contain;
        position: relative;
        bottom: 50px;
    }
    
    .footerList {
        display: flex;
        flex-direction: column;
        flex-wrap: wrap;
        width: 50%;
        height: 25rem;
        margin-left: 200px;
    }
    
    .footerList ul {
        width: 15%;
    }
    
    .footerList li {
        color: white;
        list-style: none;
    }
    
    .footerList h3 {
        color: white;
    }
    
    .signUp {
        color: white;
        background-color: #303030;
        border-color: #0282f9;
        padding: 15px;
    }
    
    .containerS3 {
        padding: 50px 30px 0px ;
        display: flex;
        justify-content: space-between;
    }
    
    .followUs {
        color:#0282f9;
    }
    
    .icone {
        margin:5px;
    }
    
    .blueBar {
        display: flex;
        justify-content: center;
        text-align: center;
        padding: 50px;
    }
</style>