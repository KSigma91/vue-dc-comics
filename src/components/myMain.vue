<template>
    <main>
        <ul>
            <li>
                <a href="#">
                    <img src="../assets/buy-comics-digital-comics.png" alt="comics_digital_img">
                    <span>DIGITAL COMICS</span>
                </a>
            </li>
            <li>
                <a href="#">
                    <img src="../assets/buy-comics-merchandise.png" alt="comics_merchandise_img">
                    <span>DC MERCHANDISE</span>
                </a>
            </li>
            <li>
                <a href="#">
                    <img src="../assets/buy-comics-subscriptions.png" alt="comics_subscriptions_img">
                    <span>SUBSCRIPTION</span>
                </a>
            </li>
            <li>
                <a href="#">
                    <img src="../assets/buy-comics-shop-locator.png" alt="comics_shop_img">
                    <span>COMIC SHOP LOCATOR</span>
                </a>
            </li>
            <li>
                <a href="#">
                    <img src="../assets/buy-dc-power-visa.svg" alt="power_visa_img">
                    <span>DC POWER VISA</span>
                </a>
            </li>
        </ul>
    </main>
</template>

<script>
    export default {
        name : 'myMain',
    }
</script>

<style scoped lang="scss">
    main {
        display: flex;
        width: 100%;
        height: 153px;
        background: #1a75f2;

        ul {
            display: flex;
            justify-content: space-evenly;
            align-items: center;
            margin: 0 auto;
            width: 80%;

            li {
                display: flex;
                justify-content: space-around;
                list-style-type: none;
                padding: 40px;

                a {
                    display: flex;
                    align-items: center;
                    text-decoration: none;
                    color: white;
                        
                    img {
                        max-width: 100%;
                        height: 55px; 
                        margin: 0 10px;
                    }
                }
            }
        }
    }
</style>