<template>
    <div class="card-area">
        <img :src="details.thumb" :alt="details.series">
    </div>
</template>

<script>
    export default {
        name : 'myThumbnail',
        props: {
            details: Object
        }
    }
</script>

<style scoped lang="scss">
    .card-area {
        display: flex;
        flex-basis: 60%;
        flex-wrap: wrap;
        justify-content: space-around;
        align-items: center;
        margin: 0 auto;
        max-width: 60%;
        //height: 90%;
            .card {
                width: 183px;
                height: 180px;
                margin: 30px 3px;

                img {
                    width: 100%;
                    max-height: 180px;
                    object-fit: cover;
                }
            }
    }
</style>