<script>
export default {
    name: 'AppHeader',
    data() {
        return {
            menu: [
                {
                    label: 'Characters',
                    selected: false
                },
                {
                    label: 'Comics',
                    selected: true
                },
                {
                    label: 'Movies',
                    selected: false
                },
                {
                    label: 'Tv',
                    selected: false
                },
                {
                    label: 'Games',
                    selected: false
                },
                {
                    label: 'Collectibles',
                    selected: false
                },
                {
                    label: 'Videos',
                    selected: false
                },
                {
                    label: 'Fans',
                    selected: false
                },
                {
                    label: 'News',
                    selected: false
                },
                {
                    label: 'Shop',
                    selected: false
                },

            ]
        }
    }
}
</script>
<template lang="">
    <header>
        <div class="container d-flex menu">
            <img src="../assets/img/dc-logo.png" alt="" class="logo">
            <ul class="d-flex">
                <li class="list" v-for="(link,index) in menu" :key="index" :class="link.selected == true ? 'selected' : ''">{{link.label}}</li>
            </ul>
        </div>
    </header>
</template>
<style lang="scss">
@use '../styles/partials/variables' as *;

header {
    margin: 20px 0;
}

.menu {
    align-items: center;
    justify-content: space-between;
}

ul {
    list-style: none;
}

.list {
    padding: 0 15px;
    text-transform: $upper;
    font-size: small;
}

.logo {
    height: 75px;
}

.selected {
    color: $primary;
}
</style>