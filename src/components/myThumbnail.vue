<template>
    <div class="card">
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
</style>