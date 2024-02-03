<script>
export default {
    name: 'AppMain',
    data() {
        return {

        }
    }
}
</script>

<template>
    <main>
        <div class="main-top">
            <div class="container">
                <span>Content goes here</span>
            </div>
        </div>
        <div class="main-bottom">
            <div class="container">
                <ul>
                    <li>
                        <img src="../assets/img/buy-comics-digital-comics.png" alt="digital-comics">
                        <span>Digital comics</span>
                    </li>
                    <li>
                        <img src="../assets/img/buy-comics-merchandise.png" alt="digital-comics">
                        <span>Dc merchandise</span>
                    </li>
                    <li>
                        <img src="../assets/img/buy-comics-shop-locator.png" alt="digital-comics">
                        <span>Subscription</span>
                    </li>
                    <li>
                        <img src="../assets/img/buy-comics-subscriptions.png" alt="digital-comics">
                        <span>Comic shop locator</span>
                    </li>
                    <li>
                        <img src="../assets/img/buy-dc-power-visa.svg" alt="digital-comics">
                        <span>Dc power visa</span>
                    </li>
                </ul>
            </div>
        </div>
    </main>
</template>


<style scoped>
.main-top {
    display: flex;
    min-height: 100px;
    background-color: var(--dc-dark);

    & span {
        color: var(--dc-white);
        align-items: center;
        font-weight: 600;
    }
}

.main-bottom {
    background-color: var(--dc-primary);
    display: flex;
    padding: 2rem 0;

    & ul {
        display: flex;
        list-style: none;
        justify-content: center;
        gap: 3rem;
        align-items: center;

        & li {
            display: flex;
            align-items: center;

            & img {
                width: 35px;
            }
        }

        & span {
            vertical-align: middle;
            padding-left: 1rem;
            color: var(--dc-white);
            text-transform: uppercase;
            font-size: 12px;
        }
    }
}
</style>