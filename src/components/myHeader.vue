<template>
    <header>
        <img src="../assets/dc-logo.png" alt="dc_logo_img">
        <nav>
            <ul>
                <li v-for="(link, i) in links" :key="i">
                    <a :href="link.url">
                        {{ link.text }}
                    </a>
                </li>
                <!-- <li>
                    <a href="#">
                        TEST
                    </a>
                </li>
                <li>
                    <a href="#">
                        TEST
                    </a>
                </li>
                <li>
                    <a href="#">
                        TEST
                    </a>
                </li>
                <li>
                    <a href="#">
                        TEST
                    </a>
                </li>
                <li>
                    <a href="#">
                        TEST
                    </a>
                </li>
                <li>
                    <a href="#">
                        TEST
                    </a>
                </li>
                <li>
                    <a href="#">
                        TEST
                    </a>
                </li>
                <li>
                    <a href="#">
                        TEST
                    </a>
                </li>
                <li>
                    <a href="#">
                        TEST
                    </a>
                </li> -->
            </ul>
        </nav>
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
                    },
                    {
                        text : "SHOP",
                        url : "#",
                        current : false
                    },
                ]
            }
        }
    }
</script>

<style scoped lang="scss">
    header {
        display: flex;
        justify-content: space-around;
        align-items: center;
        width: 100%;
        height: 140px;
        // debug
        background: grey;

        img {
            max-width: 100%;
            height: 90px;
        }

        ul {
            display: flex;
            justify-content: space-evenly;
            list-style-type: none;

            li {
                padding: 60px 20px;

                a {
                    text-decoration: none;
                    font-weight: 600;
                    color: #404a5c;
                }
            }
        }
    }
</style>