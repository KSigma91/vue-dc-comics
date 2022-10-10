<template>
    <header>
        <div class="top-header">
            <a href="#">
                DC POWER<sup>sm</sup> VISA&reg;
            </a>
            <a href="#">
                ADDITIONAL DC SITES
                <i class="fas fa-caret-down"></i>
            </a>
        </div>
        <div class="navbar">
            <img src="../assets/dc-logo.png" alt="dc_logo_img">
            <nav>
                <ul>
                    <li v-for="(link, i) in links" :key="i">
                        <a :href="link.url" :class="link.current ? 'click' : ''">
                            {{ link.text }}                     
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            SHOP
                            <i class="fas fa-caret-down"></i>
                        </a>
                    </li>
                </ul>
            </nav>
            <div>
                <input type="search" placeholder="Search">
                <i class="fas fa-search"></i>
            </div>
        </div>
    </header>
</template>

<script>
    export default {
        name : 'myHeader',
        data() {
            return {
                links : [
                    {
                        text : "CHARACTERS",
                        url : "#",
                        current : false
                    },
                    {
                        text : "COMICS",
                        url : "#",
                        current : false
                    },
                    {
                        text : "MOVIES",
                        url : "#",
                        current : false
                    },
                    {
                        text : "TV",
                        url : "#",
                        current : false
                    },
                    {
                        text : "GAMES",
                        url : "#",
                        current : false
                    },
                    {
                        text : "COLLECTIBLES",
                        url : "#",
                        current : false
                    },
                    {
                        text : "VIDEOS",
                        url : "#",
                        current : false
                    },
                    {
                        text : "FANS",
                        url : "#",
                        current : false
                    },
                    {
                        text : "NEWS",
                        url : "#",
                        current : false
                    }
                ]
            }
        }
    }
</script>

<style scoped lang="scss">
    header {
        .top-header {
            display: flex;
            justify-content: flex-end;
            align-items: center;
            gap: 54px;
            padding-right: 375px;
            background: #0282f9;
            height: 23px;
            
            a {
                font-family: Arial;
                text-decoration: none;
                color: #fff;
                font-size: .6em;
            }
        }

        .navbar {
            display: flex;
            justify-content: space-evenly;
            align-items: center;
            margin: 0 auto;
            padding: 0 100px;
            width: 80%;
            height: 86px;

            img {
                width: 60px;
            }

            ul {
                display: flex;
                justify-content: space-evenly;
                list-style-type: none;

                li {
                    padding: 60px 20px;
                
                    a {
                        text-decoration: none;
                        font-size: 1em;
                        font-weight: 500;
                        color: #404a5c;

                        &:hover {
                            padding-bottom: 27px;
                            border-bottom: 5px solid #1A75F2;
                            color: #1A75F2;
                        }
                    }
                }
            }

            div {
                border-bottom: 2px solid #1A75F2;

                input {
                    width: 110px;
                    font-family: Teko;
                    font-size: 1em;
                    font-weight: 500;
                    text-align: right;
                    outline: 0;
                    border: 0;
                }
            }
        }
    }
</style>