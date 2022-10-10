<template>
    <main>
        <ul>
            <li v-for="(icon, i) in icons" :key="i">
                <a :href="icon.url">
                    <img :src="icon.img" :alt="icon.alt">
                    <span>{{ icon.text }}</span>
                </a>
            </li>
        </ul>
    </main>
</template>

<script>
export default {
    name : 'myMain',
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
            ]
        }
    }
}
</script>

<style scoped lang="scss">
    main {
        display: flex;
        // width: 100%;
        height: 135px;
        background: #1a75f2;
        
        ul {
            display: flex;
            justify-content: center;
            gap: 15px;
            // align-items: center;
            // margin: 0 auto;
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
</style>