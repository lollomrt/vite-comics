<script>

export default {
    props: {
        serie: Object
    }
}
</script>

<template lang="">
    <div class="card">
        <img :src="serie.thumb" alt="">
        <h3>{{ serie.series }}</h3>
    </div>
</template>

<style lang="scss" scoped>
.card {
    width: calc(1200px / 6 - 1rem);
    padding: 1rem 0;

    img {
        width: calc(1200px / 6 - 1rem);
        height: calc(1200px / 6 - 1rem);
        object-fit: cover;
        object-position: top;
    }

    h3 {
        color: #fff;
        text-transform: uppercase;
        font-size: 0.9rem;
        font-weight: 400;
        margin-top: 1rem;
    }
}
</style>