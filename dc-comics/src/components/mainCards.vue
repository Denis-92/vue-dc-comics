<template>
    <div class="card">
        <img :src="card.thumb" :alt="card.series">
        <div class="title"> {{ card.series }} </div>
    </div>
</template>

<script>
export default {
    name: 'mainCards',
    props: {
        card: Object
    },
}
</script>

<style lang="scss" scoped>
.card {
    padding: 18px;
    display: flex;
    flex-direction: column;

    .title {
        text-transform: uppercase;
        padding-top: 12px;
    }

    img {
        object-fit: cover;
        object-position: top;
        height: 185px;
    }
}
</style>