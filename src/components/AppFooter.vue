<script>
export default {
    name: 'AppFooter',
    data() {
        return {

        }
    }
}
</script>
<template lang="">
    <footer>
        <div class="top d-flex container">
            <div>
                <h4>DC COMICS</h4>
                    <ul>
                        <li>Characters</li>
                        <li>Comics</li>
                        <li>Movies</li>
                        <li>Tv</li>
                        <li>Games</li>
                        <li>Videos</li>
                        <li>News</li>
                    </ul>
                <h4>SHOP</h4>
                    <ul>
                        <li>Shop Dc</li>
                        <li>Shop Dc Collectibles</li>
                    </ul>
            </div>
            <div class="space">
                <h4>DC</h4>
                    <ul>
                        <li>Terms Of Use</li>
                        <li>Privacy policy(new)</li>
                        <li>Ad Choices</li>
                        <li>Advertising</li>
                        <li>Jobs</li>
                        <li>Subscriptions</li>
                        <li>Talent Workshops</li>
                        <li>CPSC Certificates</li>
                        <li>Ratings</li>
                        <li>Shop Help</li>
                        <li>Contact Us</li>
                    </ul>
            </div>
            <div>
                <h4>SITES</h4>
                    <ul>
                        <li>DC</li>
                        <li>MAD Magazine</li>
                        <li>DC Kids</li>
                        <li>DC Universe</li>
                        <li>DC Power Visa</li>
                    </ul>
            </div>
        </div>
        <div class="bottom">
            <div class="container d-flex">
                <button>SIGN-UP NOW!</button>
                <div class="socials d-flex">
                    <span>FOLLOW US</span>
                    <img src="../assets/img/footer-facebook.png" alt="facebook">
                    <img src="../assets/img/footer-twitter.png" alt="twitter">
                    <img src="../assets/img/footer-youtube.png" alt="youtube">
                    <img src="../assets/img/footer-pinterest.png" alt="pinterest">
                    <img src="../assets/img/footer-periscope.png" alt="periscope">
                </div>
            </div>
        </div>
    </footer>
</template>
<style lang="scss">
@use '../styles/partials/variables' as *;

footer {
    color: white;
    background-image: url(../assets/img/footer-bg.jpg);
    font-size: small;

    h4 {
        margin: 10px 0px;
    }
}

.top {
    padding: 40px 0;
    background-image: url(../assets/img/dc-logo-bg.png);
    background-position: right;
    background-repeat: no-repeat;

    li {
        color: grey;
    }
}

.space {
    margin: 0 30px;
}

.bottom {
    background-color: #303030;
    padding: 25px 0;

    .container {
        justify-content: space-between;
    }

    button {
        background-color: transparent;
        border-color: $primary;
        color: white;
        font-weight: $weight-700;
        padding: 12px;
    }

    span {
        color: $primary;
        font-weight: $weight-700;
        font-size: medium;
        margin-right: 5px;
    }

    img {
        padding: 0 10px;
        height: 30px;
    }
}

.socials {
    align-items: center;
}
</style>