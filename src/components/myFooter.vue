<template>
    <footer>
        <div id="footer-top">
            <div class="col">
                <div class="task-line">
                    <ul>
                        <li>
                            <h3>DC COMICS</h3>
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
                </div>
                <div class="task-line">
                    <ul>
                        <li>
                            <h3>DC</h3>
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
                            <h3>SITES</h3>
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
                    <ul>
                        <li>
                            <h3>SHOP</h3>
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
            </div>

            <img src="../assets/dc-logo-bg.png" alt="dc_logo_bg_img">
        </div>

        <div id="footer-bottom">
            <a id="sign-up" href="#">
                <span>SIGN-UP NOW!</span>
            </a>

            <ul>
                <li>
                    <a href="#">
                        <h4>FOLLOW US</h4>
                    </a>
                </li>
                <li>
                    <a href="#">
                        <img src="../assets/footer-facebook.png" alt="facebook_img">
                    </a>
                </li>
                <li>
                    <a href="#">
                        <img src="../assets/footer-twitter.png" alt="twitter_img">
                    </a>
                </li>
                <li>
                    <a href="#">
                        <img src="../assets/footer-youtube.png" alt="youtube_img">
                    </a>
                </li>
                <li>
                    <a href="#">
                        <img src="../assets/footer-pinterest.png" alt="pinterest_img">
                    </a>
                </li>
                <li>
                    <a href="#">
                        <img src="../assets/footer-periscope.png" alt="periscope_img">
                    </a>
                </li>
            </ul>
        </div>
    </footer>
</template>

<script>
    export default {
        name : 'myFooter',
    }
</script>

<style scoped lang="scss">
    footer {
        display: flex;
        flex-direction: column;
        width: 100%;

        #footer-top {
            display: flex;
            justify-content: space-around;
            background: url(../assets/footer-bg.jpg);
            background-size: cover;        
            height: calc(100vh - 506px);

            .col {
                display: flex;
                gap: 30px;
                flex-basis: 23%;
                flex-wrap: wrap;
                justify-content: flex-start;
                align-items: center;
                max-width: 30%;

                    .task-line {
                        margin: 10px;
                        max-height: 150px;
                            
                        ul {
                            list-style-type: none;
                            
                            li {
                                text-align: left;
                                line-height: 25px;

                                h3 {
                                    color: white;
                                }

                                a {
                                    text-decoration: none;
                                    color: #8c8c8c;
                                    font-size: 13px;
                                }

                                &:first-child {
                                    margin-bottom: 10px;
                                }
                            }
                        }
                    }
            } 
            img {
                max-width: 600px;
                height: 500px;
            }  
        }
        
        #footer-bottom {
            display: flex;
            justify-content: space-around;
            align-items: center;
            background: #2c2c2c;
            height: 107px;

            #sign-up {
                text-decoration: none;
                padding: 12px 15px;
                border: 2px solid #1a6dda;
                color: white;
            }

            ul {
                display: flex;
                align-items: center;
                list-style-type: none;

                li {
                    padding: 9px;

                    h4 {
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