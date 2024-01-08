<script>
export default {
    name: 'AppMain',
    data() {
        return {

        }
    }
}
</script>
<template lang="">
    <main>
        <div class="container">
            <h1>-->Content goes here<--</h1>
        </div>
        <div class="imBlue">
            <div class="container">
                <ul class="d-flex">
                    <li>item</li>
                    <li>item</li>
                    <li>item</li>
                    <li>item</li>
                    <li>item</li>
                </ul>
            </div>
        </div>
    </main>
</template>
<style lang="scss">
@use '../styles/partials/variables' as *;

main {
    background-color: black;
    color: white;
}

h1 {
    padding: 50px 0;
}

.imBlue {
    background-color: $primary;

    li {
        padding: 50px;
    }

    ul {
        justify-content: center;
        justify-content: space-between;
    }
}
</style>