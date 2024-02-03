<script>
export default {
    name: 'AppFooter',
    data() {
        return {

        }
    }
}
</script>

<template>
    <footer>
        <div class="footer-top d-flex">
            <div class="container">
                <div class="footer-left">
                    <div class="left-col">
                        <ul>
                            <span>Dc comics</span>
                            <li><a href="">Characters</a></li>
                            <li><a href="">Comics</a></li>
                            <li><a href="">Movies</a></li>
                            <li><a href="">Tv</a></li>
                            <li><a href="">Games</a></li>
                            <li><a href="">Videos</a></li>
                            <li><a href="">News</a></li>
                        </ul>
                        <ul>
                            <span>Shop</span>
                            <li><a href="">Shop dc</a></li>
                            <li><a href="">Shop dc collectibles</a></li>
                        </ul>
                    </div>
                    <div class="right-col">
                        <ul>
                            <span>Dc</span>
                            <li><a href="">Terms of use</a></li>
                            <li><a href="">Privacy policy (new)</a></li>
                            <li><a href="">Ad Choices</a></li>
                            <li><a href="">Advertising</a></li>
                            <li><a href="">Jobs</a></li>
                            <li><a href="">Subscriptions</a></li>
                            <li><a href="">Talent Workshops</a></li>
                            <li><a href="">CPSC Certificates</a></li>
                            <li><a href="">Ratings</a></li>
                            <li><a href="">Shop Help</a></li>
                            <li><a href="">Contact Us</a></li>
                        </ul>
                        <ul>
                            <span>Sites</span>
                            <li><a href="">DC</a></li>
                            <li><a href="">MAD Magazine</a></li>
                            <li><a href="">DC Kids</a></li>
                            <li><a href="">DC Universe</a></li>
                            <li><a href="">DC Power Visa</a></li>

                        </ul>
                    </div>
                </div>
                <div class="footer-right">
                    <img src="../assets/img/dc-logo-bg.png" alt="dc-logo">
                </div>
            </div>
        </div>
        <div class="footer-bottom">
            <div class="container d-flex">
                <div class="footer-bottom-left">
                    <a href="">
                        <span>Sign-up now!</span>
                    </a>
                </div>
                <div class="footer-bottom-right">
                    <span>Follow us</span>
                    <a href=""><img src="../assets/img/footer-facebook.png" alt="facebook"></a>
                    <a href=""><img src="../assets/img/footer-twitter.png" alt="twitter"></a>
                    <a href=""><img src="../assets/img/footer-youtube.png" alt="youtube"></a>
                    <a href=""><img src="../assets/img/footer-pinterest.png" alt="pinterest"></a>
                    <a href=""><img src="../assets/img/footer-periscope.png" alt="periscope"></a>
                </div>
            </div>
        </div>

    </footer>
</template>


<style scoped>
.footer-top {
    background-image: url(../assets/img/footer-bg.jpg);
    background-size: cover;
    position: relative;
}

.footer-left {
    display: flex;
    padding: 2rem 0;

    & .left-col>ul {
        list-style: none;
        padding: 0.5rem 0.5rem;

        & span {
            text-transform: uppercase;
            color: var(--dc-white);
            font-weight: bold;
            font-size: 15px;
        }

        & li>a {
            text-decoration: none;
            color: var(--dc-light-gray);
            font-size: 10px;
        }
    }

    & .right-col {
        display: flex;

        & ul {
            list-style: none;
            padding: 0.5rem 1rem;

            & span {
                text-transform: uppercase;
                color: var(--dc-white);
                font-weight: bold;
                font-size: 15px;
            }

            & li>a {
                text-decoration: none;
                color: var(--dc-light-gray);
                font-size: 10px;
            }
        }
    }
}

.footer-right>img {
    position: absolute;
    right: 200px;
    width: 35%;
    top: -75px;
    z-index: 0;
}

.footer-bottom {
    background-color: var(--dc-gray);
    position: relative;
    z-index: 2;
    padding: 3rem 0;
    justify-content: space-between;

    & .container {
        align-items: center;
        justify-content: space-between;
    }

    & .footer-bottom-left>a {
        color: var(--dc-white);
        text-transform: uppercase;
        vertical-align: middle;
        border: 2px solid var(--dc-primary);
        padding: 0.5rem;
        text-decoration: none;
    }

    & .footer-bottom-right {
        display: flex;
        justify-content: space-between;
        align-items: center;
        gap: 1rem;

        & span {
            text-transform: uppercase;
            font-weight: 600;
            color: var(--dc-primary);
        }

        & a>img {
            width: 30px;
        }
    }

}
</style>