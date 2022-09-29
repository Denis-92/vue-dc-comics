<template>
    <div>
        <div id="card-container">
            <div class="section-block">
                <div v-for="card in cards" :key="card.series">
                    <mainCards :card="card" />
                </div>
            </div>
            <div id="load-more">
                LOAD MORE
            </div>
        </div>
        <div class="shop-section">
            <div>
                <img src="@/assets/img/buy-comics-digital-comics.png" alt="Digital comics">
                <p>DIGITAL COMICS</p>
            </div>
            <div>
                <img src="@/assets/img/buy-comics-merchandise.png" alt="Comics merchandise">
                <p>DC MERCHANDISE</p>
            </div>
            <div>
                <img src="@/assets/img/buy-comics-subscriptions.png" alt="Comics subscriptions">
                <p>SUBSCRIPTION</p>
            </div>
            <div>
                <img src="@/assets/img/buy-comics-shop-locator.png" alt="Comics shop locator">
                <p>COMIC SHOP LOCATOR</p>
            </div>
            <div>
                <img src="@/assets/img/buy-dc-power-visa.svg" alt="DC power visa">
                <p>DC POWER VISA</p>
            </div>
        </div>
    </div>
</template>

<script>
import mainCards from "./mainCards.vue"

export default {
    name: "pageMain",
    props: {
        cards: Array,
    },
    mounted() {
        console.log(this.cards);
    },
    components: {
        mainCards,
    },
}
</script>

<style lang="scss" scoped>
.section-block {
    display: flex;
    align-items: center;
    flex-wrap: wrap;

    >div {
        width: calc(100% / 6);
    }
}

.shop-section {
    height: 100px;
    width: 100%;
    background-color: blue;
    color: white;
    display: flex;
    justify-content: space-around;
    align-items: center;

    div {
        height: 50%;
        display: flex;
        align-items: center;

        img {
            height: 100%;
            padding: 0 10px;
        }
    }
}

#card-container {
    background-color: black;
    color: white;
    display: flex;
    flex-direction: column;
    align-items: center;
}

#load-more {
    background-color: blue;
    padding: 5px 25px;
    margin-bottom: 20px;
    width: 20%;
    text-align: center;
}
</style>