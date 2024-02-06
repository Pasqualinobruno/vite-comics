<script>
export default {
    name: 'AppHeader',
}
</script>

<template>
    <header>
        <div class="container menu d-flex">
            <img src="../../public/dc-logo.png" alt="" class="logo">
            <ul>
                <li><a href="#">CHARACTER</a></li>
                <li><a href="#">COMICS</a></li>
                <li><a href="#">MOVIES</a></li>
                <li><a href="#">TV</a></li>
                <li><a href="#">GAMES</a></li>
                <li><a href="#">COLLECTIBLES</a></li>
                <li><a href="#">VIDEOS</a></li>
                <li><a href="#">FANS</a></li>
                <li><a href="#">NEWS</a></li>
                <li><a href="#">SHOP</a></li>
            </ul>
        </div>
    </header>
</template>

<style scoped>
header {
    background-color: var(--dc-white);

    & .menu {
        margin: 0.5rem auto;
        display: flex;
        align-items: center;
        justify-content: center;

        & a {
            text-decoration: none;
            color: var(--dc-dark);
            padding: 1rem 0.5rem;
            font-size: small;
            font-weight: bold;
        }

        & ul {
            list-style: none;
            display: flex;

        }
    }

    & .logo {
        aspect-ratio: 1;
        height: 50px;
    }

    a:hover {
        border-bottom: 2px solid blue;
    }
}
</style>
