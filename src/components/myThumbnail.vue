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
        width: 183px;
        height: 180px;
        margin: 20px 3px;

        img {
            width: 100%;
            max-height: 180px;
            object-fit: cover;
            object-position: top;
        }

        span {
            color: white;
            font-size: 12px;
            text-align: left;
        }
    }
</style>