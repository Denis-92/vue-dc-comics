<template>
    <div>
        <div class="section-block">
            <p>-- Content goes here --</p>
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
export default {
    name: "pageMain"
}
</script>

<style lang="scss" scoped>
.section-block {
    height: 100px;
    width: 100%;
    background-color: black;
    color: white;
    display: flex;
    align-items: center;
    font-size: 2rem;

    p {
        margin-left: 20%;
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
</style>