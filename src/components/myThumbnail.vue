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
        margin-bottom: 20px;

        img {
            width: 176px;
            height: 178px;
            object-fit: cover;
            object-position: top;
        }

        span {
            width: 160px;
            line-height: 1.2em;
            color: white;
            font-size: .7em;
            text-align: left;
        }
    }
</style>