<template>
    <footer>
        <div id="footer-top">
            <ul>
                <li v-for="(icon, i) in icons" :key="i">
                    <a :href="icon.url">
                        <img :src="icon.img" :alt="icon.alt">
                        <span>{{ icon.text }}</span>
                    </a>
                </li>
            </ul>
        </div>
        <div id="footer-mid">
            <div class="col">
                <div class="task-line">
                    <ul>
                        <li>
                            <h2>DC COMICS</h2>
                        </li>
                        <li>
                            <a href="#">
                                Characters
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                Comics
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                Movies
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                TV
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                Games
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                Videos
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                News
                            </a>
                        </li>
                    </ul>
                    <ul>
                        <li>
                            <h2>SHOP</h2>
                        </li>
                        <li>
                            <a href="#">
                                Shop DC
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                Shop DC Collectibles
                            </a>
                        </li>
                    </ul>
                </div>
                <div class="task-line">
                    <ul>
                        <li>
                            <h2>DC</h2>
                        </li>
                        <li>
                            <a href="#">
                                Terms Of Use
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                Privacy policy (New)
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                Ad Choices
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                Advertising
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                Jobs
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                Subscriptions
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                Talent Workshops
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                CPSC Certificates
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                Ratings
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                Shop Help
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                Contact Us
                            </a>
                        </li>
                    </ul>
                </div>
                <div class="task-line">
                    <ul>
                        <li>
                            <h2>SITES</h2>
                        </li>
                        <li>
                            <a href="#">
                                DC
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                MAD Magazine
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                DC Kids
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                DC Universe
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                DC Power Visa
                            </a>
                        </li>
                    </ul>
                </div>
                <div class="task-line">
                    <p>
                        All Site Content TM and &copy; 2020 DC Entertainment, unless otherwise <span>noted here</span>. All rights reserved. <span>Cookies Settings</span>
                    </p>
                </div>
            </div>
            <img src="../assets/dc-logo-bg.png" alt="dc_logo_bg_img">
        </div>

        <div id="footer-bottom">
            <a id="sign-up" href="#">
                SIGN-UP NOW!
            </a>
            <ul>
                <li>
                    <a href="#">
                        <h2>FOLLOW US</h2>
                    </a>
                </li>
                <li v-for="(social, i) in listSocial" :key="i">
                    <a :href="social.url">
                        <img :src="social.img" :alt="social.alt">
                    </a>
                </li>
            </ul>
        </div>
    </footer>
</template>

<script>
    export default {
        name : 'myFooter',
        data() {
            return {
                icons : [
                    {
                        url : "#",
                        img : require("../assets/buy-comics-digital-comics.png"),
                        alt : "comics_digital_img",
                        text : "DIGITAL COMICS"
                    },
                    {
                        url : "#",
                        img : require("../assets/buy-comics-merchandise.png"),
                        alt : "comics_merchandise_img",
                        text : "DC MERCHANDISE"
                    },
                    {
                        url : "#",
                        img : require("../assets/buy-comics-subscriptions.png"),
                        alt : "comics_subscriptions_img",
                        text : "SUBSCRIPTION"
                    },
                    {
                        url : "#",
                        img : require("../assets/buy-comics-shop-locator.png"),
                        alt : "comics_shop_locator_img",
                        text : "COMIC SHOP LOCATOR"
                    },
                    {
                        url : "#",
                        img : require("../assets/buy-dc-power-visa.svg"),
                        alt : "power_visa_img",
                        text : "DC POWER VISA"
                    },
                ],
                listSocial : [
                    {
                        img : require("../assets/footer-facebook.png"),
                        alt : "facebook_img",
                        url : "#",
                    },
                    {
                        img : require("../assets/footer-twitter.png"),
                        alt : "twitter_img",
                        url : "#",
                    },
                    {
                        img : require("../assets/footer-youtube.png"),
                        alt : "youtube_img",
                        url : "#",
                    },
                    {
                        img : require("../assets/footer-pinterest.png"),
                        alt : "pinterest_img",
                        url : "#",
                    },
                    {
                        img : require("../assets/footer-periscope.png"),
                        alt : "periscope_img",
                        url : "#"
                    },
                ]
            }
        }
    }
</script>

<style scoped lang="scss">
    footer {
        display: flex;
        flex-direction: column;
        width: 100%;

        #footer-top {
            display: flex;
            height: 135px;
            background: #1a75f2;
            z-index: 300;

                ul {
                display: flex;
                justify-content: center;
                gap: 15px;
                width: 100%;

                li {
                    display: flex;
                    justify-content: space-around;
                    list-style-type: none;
                    padding: 30px;

                    a {
                        display: flex;
                        align-items: center;
                        text-decoration: none;
                        font-family: Helvetica;
                        color: white;
                            
                        img {
                            object-fit: contain;
                            width: 43px;
                            height: 54px; 
                            margin-right: 10px;
                        }

                        span {
                            font-size: 13px;
                        }
                    }
                }
            }
        }

        #footer-mid {
            position: relative;
            display: flex;
            background: url(../assets/footer-bg.jpg);
            background-size: cover;        
            height: 42vh;

            .col {
                display: flex;
                flex-wrap: wrap;
                justify-content: flex-start;
                align-items: center;
                // gap: 30px;
                margin-left: 320px;
                max-width: 30%;

                .task-line {
                    margin: 10px;
                    max-height: 140px;
                            
                    ul {
                        list-style-type: none;
                        margin-bottom: 25px;
                            
                        li {
                            text-align: left;

                            h2 {
                                font-weight: 500;
                                color: white;
                            }

                            a {
                                line-height: 10px;
                                font-family: Helvetica;
                                text-decoration: none;
                                color: #8c8c8c;
                                font-size: .7em;
                            }

                            &:first-child {
                                 margin-bottom: 10px;
                            }
                        }
                    }

                    p {
                        margin-top: 80px;
                        padding-right: 30px;
                        text-align: left;
                        color: #8c8c8c;
                        font-size: .7em;

                        span {
                            color: #0282f9;
                        }
                    }
                }
            } 
            img {
                position: absolute;
                top: -15%;
                right: 18%;
                z-index: 100;
                max-width: 100%;
                height: 537px;
            }  
        }
        
        #footer-bottom {
            display: flex;
            justify-content: space-around;
            align-items: center;
            z-index: 300;
            background: #2c2c2c;
            height: 100px;

            #sign-up {
                padding: 12px 15px;
                font-family: Helvetica;
                font-size: .8em;
                text-decoration: none;
                border: 2px solid #1a6dda;
                color: white;
            }

            ul {
                display: flex;
                align-items: center;
                list-style-type: none;

                li {
                    padding: 9px;

                    h2 {
                        font-weight: 500;
                        color: #1875dd;
                    }

                    &:first-child {
                        margin-right: 10px;
                    }

                    a {
                        text-decoration: none;
                    }
                }
            }
        }
    }
</style>