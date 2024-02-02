<script>
export default {
    name: 'AppHeader',
    data() {
        return {

        }
    }
}
</script>

<template>
    <header>
        <nav>
            <div class="container">
                <div class="logo">
                    <img width="70%" src="../assets/img/dc-logo.png" alt="" srcset="">
                </div>
                <ul>
                    <li><a href="">Charachters</a></li>
                    <li>
                        <a class="active" href="">Comics</a>
                        <div class="active-box"></div>
                    </li>
                    <li><a href="">Movies</a></li>
                    <li><a href="">Tv</a></li>
                    <li><a href="">Games</a></li>
                    <li><a href="">Collectibles</a></li>
                    <li><a href="">Videos</a></li>
                    <li><a href="">Fans</a></li>
                    <li><a href="">News</a></li>
                    <li><a href="">Shop</a></li>
                </ul>
            </div>
        </nav>
    </header>
</template>


<style scoped>
header {
    min-height: 200px;
    background-color: var(--dc-white);
    padding: 1rem 0;

    & .container {
        display: flex;
        justify-content: space-between;
        align-items: center;

        & ul {
            display: flex;
            gap: 1rem;
            align-items: center;

            & li {
                list-style: none;
                padding: 2rem 0;
                position: relative;

                & a.active {
                    color: var(--dc-primary);
                }

                & .active-box {
                    position: absolute;
                    width: 100%;
                    height: 5px;
                    top: 100%;
                    background-color: var(--dc-primary);

                }

                & a {
                    text-decoration: none;
                    color: var(--dc-light);
                    font-weight: 600;
                    font-size: 12px;
                }
            }
        }
    }
}

.container {
    width: 70%;
    margin: auto;
}

a.active {
    color: var(--dc-primary);
}
</style>