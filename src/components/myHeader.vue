<template>
    <header>
        <img src="../assets/dc-logo.png" alt="dc_logo_img">
        <nav>
            <ul>
                <li v-for="(link, i) in links" :key="i">
                    <a :href="link.url" :class="link.current ? 'click' : ''">
                        {{ link.text }}                      
                    </a>
                </li>
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
        margin: 0 auto;
        width: 80%;
        height: 116px;

        img {
            max-width: 78px;
        }

        ul {
            display: flex;
            justify-content: space-evenly;
            list-style-type: none;

            li {
                padding: 60px 20px;
            
                a {
                    text-decoration: none;
                    font-size: 12px;
                    font-weight: 600;
                    color: #404a5c;

                    &:hover {
                        padding-bottom: 45px;
                        border-bottom: 5px solid #1A75F2;
                        color: #1A75F2;
                    }
                }
            }
        }
    }
</style>