<template>
    <section>
        <img src="../assets/jumbotron.jpg" alt="jumbotron_img">
    </section>
</template>

<script>
    export default {
        name : 'myJumbotron',
    }
</script>

<style scoped lang="scss">
    section {
        display: flex;
        justify-content: space-around;
        align-items: center;

        img {
            width: 100%;
            height: 368px;
            object-fit: cover;
            object-position: top;
        }

        a {
            text-decoration: none;
            width: 70%;

            h1 {
                color: white;
                text-align: left;
            }
        }
    }
</style>