<script>
export default {
    data() {
        return {
            links: [
                "characters",
                "comics",
                "movies",
                "tv",
                "games",
                "collectibles",
                "videos",
                "fans",
                "news",
                "shop"
            ],
            activeIndex: 0,
        }
    },
    methods: {
        changeActiveIndex(index) {
            this.activeIndex = index;
        }
    }
}
</script>

<template>
    <header>

        <div class="container">

            <div id="logo">
                <img src="/img/dc-logo.png" alt="">
            </div>
            <div id="links">
                <ul>

                    <li v-for="(link, index) in links" :class="activeIndex == index ? `active` : ``"
                        @click="changeActiveIndex(index)">{{ link }}</li>

                </ul>

            </div>

        </div>

    </header>
</template>

<style lang="scss" scoped>
header {
    background-color: white;
    color: black;

    .container {
        display: flex;
        flex-flow: row nowrap;
        justify-content: space-between;
        align-items: center;

        height: 100px;

        #logo {
            img {
                height: 80px;
            }
        }

        #links {
            height: 100%;
        }

        ul {
            display: flex;
            gap: 1em;
            height: 100%;

            li {
                text-transform: uppercase;
                font-weight: 500;
                display: flex;
                align-items: center;
                cursor: pointer;


            }

            li.active {
                color: #1282f9;
                border-bottom: 5px solid #1282f9;
                border-top: 5px solid white;
            }

        }
    }
}
</style>