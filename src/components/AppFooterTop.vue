<script>
export default {
    data() {
        return {
            links: [
                {
                    text: "digital comics",
                    img: "/img/buy-comics-digital-comics.png"
                },
                {
                    text: "dc merchandise",
                    img: "/img/buy-comics-merchandise.png"
                },
                {
                    text: "subscription",
                    img: "/img/buy-comics-shop-locator.png"
                },
                {
                    text: "comic shop locator",
                    img: "/img/buy-comics-subscriptions.png"
                },
                {
                    text: "dc power visa",
                    img: "/img/buy-dc-power-visa.svg"
                }
            ]
        }
    }
}
</script>

<template>
    <div id="container-wrapper">

        <div class="container">
            <ul>
                <li v-for="link in links">
                    <img :src="link.img" alt="">
                    <a href="#">{{ link.text }}</a>
                </li>

            </ul>
        </div>

    </div>
</template>

<style lang="scss" scoped>
#container-wrapper {
    background-color: #1282f8;
    height: 150px;

    .container {

        height: 100%;

        ul {
            display: flex;
            justify-content: space-around;
            align-items: center;
            gap: 1em;

            height: 100%;


            li {

                display: flex;
                align-items: center;
                gap: 1em;
                text-transform: uppercase;

                img {
                    height: 60px;
                }

                a {
                    color: white;
                }
            }
        }

    }

}
</style>