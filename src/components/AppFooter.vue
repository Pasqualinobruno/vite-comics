<script>
export default {
    name: 'AppFooter',

}
</script>
<template>
    <footer>
        <div class="top-footer">
            <div class="container">
                <div class="row">
                    <div class="col-2">
                        <h2> Dc Comics</h2>
                        <ul>
                            <li>Characters</li>
                            <li>Comics</li>
                            <li>Movies</li>
                            <li>Tv</li>
                            <li>Games</li>
                            <li>Videos</li>
                            <li>News</li>
                        </ul>
                        <h2>shop</h2>
                        <ul>
                            <li>Shop Dc</li>
                            <li>Shop Dc Collectibles</li>
                        </ul>
                    </div>
                    <div class="col-2">
                        <h2>dc</h2>
                        <ul>
                            <li>Terms Of Use</li>
                            <li>Privacy policy (New)</li>
                            <li>Ad Choices</li>
                            <li>Advertising</li>
                            <li>Jobs</li>
                            <li>Subscriptions</li>
                            <li>Talent Workshops</li>
                            <li>CPSC Certificstes</li>
                            <li>Ratings</li>
                            <li>Shop Help</li>
                            <li>Contact Us</li>
                        </ul>
                    </div>
                    <div class="col-2 sites">
                        <h2>sites</h2>
                        <ul>
                            <li>DC</li>
                            <li>MAD Magazine</li>
                            <li>DC Kids</li>
                            <li>DC Universe</li>
                            <li>DC Power Visa</li>
                        </ul>
                    </div>
                    <div class="col-6"></div>
                </div>
            </div>
        </div>
        <div class="under-footer">
            <div class="container">
                <div class="row">
                    <col-6><button class="btn">Sign-up now!</button></col-6>
                    <col-6 class="follow">
                        <h3>Follow us</h3>
                        <img src="../../public/footer-facebook.png" alt="">
                        <img src="../../public/footer-twitter.png" alt="">
                        <img src="../../public/footer-youtube.png" alt="">
                        <img src="../../public/footer-pinterest.png" alt="">
                        <img src="../../public/footer-periscope.png" alt="">
                    </col-6>
                </div>
            </div>
        </div>
    </footer>
</template>
<style scoped>
.top-footer {
    background-color: aquamarine;
    background-image: url(../public/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    min-height: 400px;
    padding: 1rem;

    & h2 {
        color: var(--dc-white);
        text-transform: uppercase;
    }

    & ul {
        margin: 1rem auto;

        & li {
            list-style: none;
            color: var(--dc-gray);
            padding: 0.25rem 0;
            font-size: x-small;
        }
    }
}

.sites {
    margin-top: initial;
}

.under-footer {
    padding: 1rem 0;
    background-color: var(--dc-footer-gray);
    font-size: small;
}

.follow {
    display: flex;
    gap: 1rem;

    & h3 {
        color: blue;
    }
}

.btn {
    border-color: blue;
    padding: 0.5rem 1rem;
    background-color: transparent;
    color: var(--dc-white);
}
</style>