<template>
    <div>
        <div class="header-container">
            <div id="logo">
                <img src="../assets/img/dc-logo.png" alt="DC Logo">
            </div>
            <nav>
                <div id="navigation-menu">
                    <div class="menu-component" v-for="nav in navigation" :key="nav.menu" :class="{active: nav.active}">
                        {{ nav.menu }} </div>
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
                    active: false,
                },
                {
                    menu: 'COMICS',
                    active: true,
                },
                {
                    menu: 'MOVIES',
                    active: false,
                },
                {
                    menu: 'TV',
                    active: false,
                },
                {
                    menu: 'GAMES',
                    active: false,
                },
                {
                    menu: 'COLLECTIBLES',
                    active: false,
                },
                {
                    menu: 'VIDEOS',
                    active: false,
                },
                {
                    menu: 'FANS',
                    active: false,
                },
                {
                    menu: 'NEWS',
                    active: false,
                },
                {
                    menu: 'SHOP',
                    active: false,
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
    height: 100%;
}

.menu-component {
    font-size: 1.2rem;
    padding: 5px;
    height: 100%;
    display: flex;
    align-items: center;
}

.active {
    color: blue;
    border-bottom: 5px solid blue;
    padding-bottom: 0;
}
</style>