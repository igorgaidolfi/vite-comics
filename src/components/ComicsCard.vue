<script>
export default {
    name: 'ComicsCard',
    props: {
        series: Object
    }
}
</script>
<template lang="">
    <div class="card">
        <img :src="series.thumb" alt="series.series">
        <p>{{series.series}}</p>
    </div>
</template>
<style lang="scss" scoped>
.card {
    width: calc(100%/6);

    img {
        height: 200px;
        width: 200px;
        margin: 50px 0px 15px 0px;
    }

    p {
        text-transform: uppercase;
        margin-bottom: 10px;
    }
}
</style>