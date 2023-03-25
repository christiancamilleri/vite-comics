<script>
export default {
    data() {
        return {
            srcImg: [
                "/img/footer-facebook.png",
                "/img/footer-periscope.png",
                "/img/footer-pinterest.png",
                "/img/footer-twitter.png",
                "/img/footer-youtube.png"
            ]
        }
    }
}
</script>

<template>
    <div class="container">
        <div id="footer-left">

            <button>Sign Up Now!</button>

        </div>
        <div id="footer-right">

            <strong>Follow Us</strong>
            <a v-for="src in srcImg" href="#">
                <img :src="src" alt="">
            </a>




        </div>
    </div>
</template>

<style lang="scss" scoped>
.container {
    display: flex;
    justify-content: space-between;
    align-items: center;

    padding: 1em 0;

    #footer-left {
        button {
            padding: 10px;
            border-color: #1282f9;
            cursor: pointer;
        }
    }

    #footer-right {
        display: flex;
        align-items: center;
        gap: 15px;

        strong {
            text-transform: uppercase;
            color: #1282f9;
        }
    }
}
</style>