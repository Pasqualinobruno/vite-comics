<script>
import AppJunbotron from './AppJunbotron.vue';
export default {
    name: 'AppMain',
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
    },
    components: {
        AppJunbotron,

    }
}
</script>
<template>
    <main>
        <AppJunbotron></AppJunbotron>
        <section class="top-main">

            <div class="container">
                <h3>Current Series</h3>
                <div class="row">
                    <div class="col-2" v-for="comic in comics">
                        <div class="card">
                            <img :src="comic.thumb" alt="">
                            <h4>{{ comic.series }}</h4>
                        </div>
                    </div>
                    <button class="btn">Load More</button>
                </div>
            </div>
        </section>
        <div class="under-main">
            <div class="container d-flex">
                <ul>
                    <li><a href="#"><img src="../../public/buy-comics-digital-comics.png" alt="">Digital Comics</a></li>
                    <li><a href="#"><img src="../../public/buy-comics-merchandise.png" alt="">DC Merchandise</a></li>
                    <li><a href="#"><img src="../../public/buy-comics-subscriptions.png" alt="">subscription</a></li>
                    <li><a href="#"><img src="../../public/buy-comics-shop-locator.png" alt="">comic shop locator</a></li>
                    <li><a href="#"><img src="../../public/buy-dc-power-visa.svg" alt="">dc power visa</a></li>
                </ul>
            </div>
        </div>
    </main>
</template>

<style scoped>
.top-main {
    background-color: var(--dc-dark);
    padding-bottom: 1rem;

    & .container {
        display: ;
    }

    & img {
        aspect-ratio: 1;
        object-fit: cover;
        object-position: top;
        height: 200px;

    }

    & .col-2 {
        margin-top: 1rem;
    }

    & h3 {
        display: inline-block;
        background-color: var(--dc-primary);
        padding: 0.5rem 1.5rem;
        margin: -2rem -1rem 0 -1rem;
        color: var(--dc-white);
    }

    & h4 {
        color: var(--dc-white);
        text-align: initial;
        font-size: small;
    }
}

a {
    text-decoration: none;
    color: var(--dc-white);
}

.under-main {
    background-color: var(--dc-primary);
    min-height: 100px;
    padding: 2rem;



    & ul {
        display: flex;
        gap: 2rem;
        list-style: none;
        align-items: center;

        & img {
            height: 40px;
        }

        & li,
        a {
            display: flex;
            align-items: center;
            gap: 0.5rem;
            text-transform: uppercase;
            color: var(--dc-white);
            font-size: small;

        }
    }
}

.btn {
    padding: 0.5rem 2rem;
    background-color: var(--dc-primary);
    color: var(--dc-white);
    margin-top: 1rem
}

.card:hover {
    opacity: 0.3;
}
</style>