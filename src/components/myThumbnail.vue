<template>
    <div class="card">
        <img :src="details.thumb" :alt="details.series">
        <span>{{ details.series}}</span>
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
    .card {
        display: flex;
        flex-wrap: wrap;
        flex-direction: column;
        gap: 15px;
        margin-bottom: 25px;

        img {
            width: 118px;
            height: 120px;
            object-fit: cover;
            object-position: top;
        }

        span {
            width: 130px;
            color: white;
            font-size: .6em;
            text-align: left;
        }
    }
</style>