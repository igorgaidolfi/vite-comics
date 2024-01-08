<script>
export default {
    name: 'AppHeader',
    data() {
        return {

        }
    }
}
</script>
<template lang="">
    <header>
        <div class="container d-flex">
            <img src="../assets/img/dc-logo.png" alt="">
            <ul>
                <li>Characters</li>
                <li>Comics</li>
                <li>Movies</li>
                <li>Tv</li>
                <li>Games</li>
                <li>Collectibles</li>
                <li>Videos</li>
                <li>Fans</li>
                <li>News</li>
                <li>Shop</li>
            </ul>
        </div>
    </header>
</template>
<style lang="scss">
header {
    margin: 20px 0;
}

.d-flex {
    display: flex;
    align-items: center;
    justify-content: space-between;
}

ul {
    display: flex;
    list-style: none;
}

li {
    padding: 0 15px;
}

img {
    height: 75px;
}
</style>