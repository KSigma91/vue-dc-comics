<template>
    <header>
        <img src="../assets/dc-logo.png" alt="dc_logo_img">
        <nav>
            <ul>
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

            </ul>
        </nav>
    </header>
</template>

<script>
    export default {
        name : 'myHeader',
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
            height: 100px;
        }

        ul {
            display: flex;
            justify-content: space-evenly;
            list-style-type: none;

            li {
                padding: 60px 20px;

                a {
                    text-decoration: none;
                    color: #404a5c;
                }
            }
        }
    }
</style>