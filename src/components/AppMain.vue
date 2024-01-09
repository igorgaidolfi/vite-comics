<script>
import ComicsCard from './ComicsCard.vue';
export default {
    name: 'AppMain',
    components: {
        ComicsCard
    },
    data() {
        return {
            comics: [
                {
                    "thumb": "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book",
                },
                {
                    "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book",
                },
                {
                    "thumb": "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel",
                },
                {
                    "thumb": "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel",
                },
            ]
        }
    }
}
</script>
<template lang="">
    <main>
        <div class="jumbotron">

        </div>
        <div class="container">
            <div class="comic-container d-flex">
                <span class="blue-label">current series</span>
                <ComicsCard v-for="comic, index in comics" :key="index" :series="comic"/>
                <button class="blue-button">load more</button>
            </div>
        </div>
        <div class="blueBanner">
            <div class="container">
                <div class="d-flex">
                    <div class="item d-flex">
                        <img src="../assets/img/buy-comics-digital-comics.png" alt="digital-comics">
                        <span>digital comics</span>
                    </div>
                    <div class="item d-flex">
                        <img src="../assets/img/buy-comics-merchandise.png" alt="merchandise">
                        <span>dc merchandise</span>
                    </div>
                    <div class="item d-flex">
                        <img src="../assets/img/buy-comics-subscriptions.png" alt="subscription">
                        <span>subscription</span>
                    </div>
                    <div class="item d-flex">
                        <img src="../assets/img/buy-comics-shop-locator.png" alt="comic-shop-locator">
                        <span>comic shop locator</span>
                    </div>
                    <div class="item d-flex">
                        <img src="../assets/img/buy-dc-power-visa.svg" alt="dc-power-visa">
                        <span>dc power visa</span>
                    </div>
                </div>
            </div>
        </div>
    </main>
</template>
<style lang="scss">
@use '../styles/partials/variables' as *;

main {
    background-color: black;
    color: white;
}

.jumbotron {
    background-image: url(../assets/img/jumbotron.jpg);
    height: 420px;
    background-size: cover;

}

.comic-container {
    flex-wrap: wrap;
    position: relative;

    .blue-label {
        background-color: $primary;
        position: absolute;
        text-transform: $upper;
        font-size: x-large;
        font-weight: $weight-700;
        padding: 10px 20px;
        top: -27px;
        left: 0
    }

    .blue-button {
        background-color: $primary;
        margin: 40px auto 20px auto;
        text-transform: $upper;
        padding: 10px 60px;
        color: white;
        border: 0px;
        font-weight: $weight-700;


    }
}

.blueBanner {
    background-color: $primary;

    .d-flex {
        justify-content: space-between;
        align-items: center;
    }

    .item {
        padding: 50px 20px;
        align-items: center;


        img {
            width: 50px;
            margin-right: 10px;
        }

        span {
            text-transform: $upper;
        }
    }
}
</style>