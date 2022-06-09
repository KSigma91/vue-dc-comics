<template>
    <section>
        <a href="#">
            <h1>Content goes here</h1>
        </a>
    </section>
</template>

<script>
    export default {
        name : 'calltoAction',
    }
</script>

<style scoped lang="scss">
    section {
        display: flex;
        justify-content: space-around;
        align-items: center;
        background: #1b1b1b;
        width: 100%;
        height: 130px;

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