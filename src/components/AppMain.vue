<script>

import AppMainBottom from './AppMainBottom.vue';
import AppBooks from './AppBooks.vue';


export default {
    name: 'AppMain',
    data() {
        return {
            books: [
                {
                    thumb: "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
                    price: "$19.99",
                    series: "Action Comics",
                    type: "comic book"
                },
                {
                    thumb: "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
                    price: "$3.99",
                    series: "American Vampire 1976",
                    type: "comic book"
                },
                {
                    thumb: "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
                    price: "$16.99",
                    series: "Aquaman",
                    type: "graphic novel"
                },
                {
                    thumb: "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
                    price: "$2.99",
                    series: "Batgirl",
                    type: "comic book"
                },
                {
                    thumb: "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
                    price: "$3.99",
                    series: "Batman",
                    type: "comic book"
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
                    price: "$2.99",
                    series: "Batman Beyond",
                    type: "comic book"
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
                    price: "$3.99",
                    series: "Batman/Superman",
                    type: "comic book"
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
                    price: "$4.99",
                    series: "Batman/Superman Annual",
                    type: "comic book"
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
                    price: "$5.99",
                    series: "Batman: The Joker War Zone",
                    type: "comic book"
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
                    price: "$6.99",
                    series: "Batman: Three Jokers",
                    type: "comic book"
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
                    price: "$4.99",
                    series: "Batman: White Knight Presents: Harley Quinn",
                    type: "comic book"
                },
                {
                    thumb: "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
                    price: "$16.99",
                    series: "Catwoman",
                    type: "graphic novel"
                }
            ]
        };
    },
    components: {
        AppMainBottom,
        AppBooks
    }
}
</script>

<template>
    <main>
        <div class="main-top">
            <div class="jumbotron"></div>
            <div class="container">
                <span>Current Series</span>
            </div>

            <div class="books">
                <div class="container">
                    <div class="row">
                        <div class="col-2" v-for="book in books">
                            <AppBooks :src="book.thumb" :text="book.type"></AppBooks>
                        </div>
                    </div>
                </div>
            </div>
            <div class="load">
                <button>Load more</button>
            </div>
        </div>
        <AppMainBottom></AppMainBottom>
    </main>
</template>


<style scoped>
.main-top {
    min-height: 100px;
    background-color: var(--dc-dark);

    & .container>span {
        color: var(--dc-white);
        align-items: center;
        font-weight: 600;
        text-transform: uppercase;
        background-color: var(--dc-primary);
        padding: 0.5rem 1rem;
    }

    & .jumbotron {
        background-image: url(../assets/img/jumbotron.jpg);
        background-size: cover;
        background-repeat: no-repeat;
        height: 300px;
        max-width: 100%;
    }
}

.books {
    background-color: var(--dc-dark);
    padding: 1rem;

}

.row {
    display: flex;
    flex-wrap: wrap;

}

.col-2 {
    width: calc(100% / 12 * 2);
    padding: 0.5rem 1rem
}

.load {
    text-align: center;
    padding-bottom: 1.5rem;

    & button {
        color: var(--dc-white);
        font-weight: 600;
        text-transform: uppercase;
        padding: 0.5rem 2rem;
        background-color: var(--dc-primary);
        border-style: none;

    }
}
</style>