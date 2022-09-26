<template>
    <div class="section-container">
        <div class="header-container">
            <div id="logo">
                <img src="../assets/img/dc-logo.png" alt="DC Logo">
            </div>
            <nav>
                <div id="navigation-menu">
                    <div class="menu-component" v-for="nav in navigation" :key="nav.menu"> {{ nav.menu }} </div>
                </div>
            </nav>

        </div>
    </div>
</template>

<script>
export default {

    name: "pageHeader",

    data() {
        return {
            navigation: [
                {
                    menu: 'CHARACTERS',
                },
                {
                    menu: 'COMICS',
                },
                {
                    menu: 'MOVIES',
                },
                {
                    menu: 'TV',
                },
                {
                    menu: 'GAMES',
                },
                {
                    menu: 'COLLECTIBLES',
                },
                {
                    menu: 'VIDEOS',
                },
                {
                    menu: 'FANS',
                },
                {
                    menu: 'NEWS',
                },
                {
                    menu: 'SHOP',
                },
            ]
        }
    }
};
</script>

<style lang="scss" scoped>
.header-container {
    display: flex;
    justify-content: space-between;
}

#navigation-menu {
    display: flex;
}

.menu-component {
    font-size: 0.7rem;
    padding: 5px;
}
</style>