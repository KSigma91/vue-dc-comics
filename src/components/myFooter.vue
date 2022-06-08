<template>
    <footer>
        <div id="footer-top">
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
        height: calc(100vh - 423px);
        width: 100%;

        #footer-top {
            display: flex;
            justify-content: space-around;
            background: url(../assets/footer-bg.jpg);
            background-size: cover;
            width: 100%;
            height: calc(100vh - 423px);

            .task-line {
                display: flex;
                justify-content: center;
                        
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
                            color: #716b66;
                            font-size: 15px;
                        }
                    }
                }
            }

            img {
                max-width: 600px;
                height: 600px;
            }
        }   
        
        #footer-bottom {
            display: flex;
            justify-content: space-around;
            align-items: center;
            background: #2c2c2c;
            width: 100%;
            height: 104px;

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
                    padding: 8px;

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