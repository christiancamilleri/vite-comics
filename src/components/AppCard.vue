<script>
export default {
    data() {
        return {

        }
    },
    props: {
        img: String,
        title: String,
    }
}
</script>

<template>
    <div class="card">
        <div class="img-container">
            <img :src="img" alt="">
        </div>
        <div id="title">{{ title }}</div>
    </div>
</template>

<style lang="scss" scoped>
.card {
    width: calc(100% / 6 - 30px);
    margin-bottom: .8em;

    .img-container {
        border: 1px solid white;
        height: 190px;
        width: 190px;

        overflow: hidden;


        img {
            width: 100%;
            object-fit: contain;

        }

    }

    #title {
        font-size: .8em;
        text-transform: uppercase;
        padding: .5em 0;
    }

}
</style>