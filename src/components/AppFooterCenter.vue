<script>
export default {
    data() {
        return {
            lists: [
                {
                    titolo: "dc comics",
                    links: [
                        "Characters",
                        "Comics",
                        "Movies",
                        "TV",
                        "Games",
                        "Videos",
                        "News"
                    ]
                },
                {
                    titolo: "shop",
                    links: [
                        "Shop DC",
                        "Shop DC collectibles"
                    ]
                },
                {
                    titolo: "dc",
                    links: [
                        "Terms Of Use",
                        "Privacy Policy(New)",
                        "Ad Choices",
                        "Advertising",
                        "Jobs",
                        "Subscriptions",
                        "Talent Workshops",
                        "CPSC Certificates",
                        "Ratings",
                        "Shop Help",
                        "Contact Us"
                    ]
                },
                {
                    titolo: "sites",
                    links: [
                        "DC",
                        "MAD Magazine",
                        "DC Kids",
                        "DC Universe",
                        "DC Power Visa"
                    ]
                },
            ]
        }
    }
}
</script>

<template>
    <div class="container-wrapper">

        <div class="container">
            <div id="list-container">
                <div v-for="list in lists">
                    <h2>{{ list.titolo }}</h2>
                    <ul>
                        <li v-for="link in list.links">
                            <a href="#">{{ link }}</a>
                        </li>
                    </ul>
                </div>

            </div>
            <div id="img-container">
                <img src="/img/dc-logo-bg.png" alt="">
            </div>

        </div>
    </div>
</template>

<style lang="scss" scoped>
.container-wrapper {
    background-image: url("/img/footer-bg.jpg");
    background-repeat: no-repeat;
    background-size: cover;

    .container {
        display: flex;
        justify-content: space-between;

        height: 400px;

        #list-container {
            width: 400px;
            height: 100%;
            display: flex;
            flex-flow: column wrap;
            gap: 1em;

            padding: 50px 0;

            h2 {
                text-transform: uppercase;
                margin-bottom: .5em;
                font-size: 1.3em;


            }

            ul {
                li {
                    font-size: .8rem;
                    opacity: .6;

                    a {
                        color: white;
                    }
                }
            }
        }

        #img-container {
            height: 100%;

            display: flex;
            align-items: center;

            overflow: hidden;

        }
    }

}
</style>