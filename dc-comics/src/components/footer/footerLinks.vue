<template>
    <div id="mid-section-footer">

        <div id="footer-links-container">

            <div class="column">
                <div class="title">DC COMICS</div>
                <div>Characters</div>
                <div>Comics</div>
                <div>Movies</div>
                <div>TV</div>
                <div>Games</div>
                <div>Videos</div>
                <div>News</div>
            </div>
            <div class="column">
                <div class="title">DC</div>
                <div>Terms Of Use</div>
                <div>Privacy policy (New)</div>
                <div>Ad Choices</div>
                <div>Advertising</div>
                <div>Jobs</div>
                <div>Subscriptions</div>
                <div>Talent Workshops</div>
                <div>CPSC Certificates</div>
                <div>Ratings</div>
                <div>Shop Help</div>
                <div>Contact Us</div>
            </div>
            <div class="column">
                <div class="title">SITES</div>
                <div>DC</div>
                <div>MAD Magazine</div>
                <div>DC Kids</div>
                <div>DC Universe</div>
                <div>DC Power Visa</div>
            </div>

            <div class="column">
                <div class="title">SHOP</div>
                <div>Shop DC</div>
                <div>Shop DC Collectibles</div>
            </div>

        </div>

        <div id="logo-container">
            <img src="../../assets/img/dc-logo-bg.png" alt="DC Logo background">
        </div>

    </div>
</template>

<script>
export default {
    name: "footerLinks"
}
</script>

<style lang="scss" scoped>
#footer-links-container {

    display: flex;
    padding: 15px;
    width: 50%;
    flex-wrap: wrap;
}

#mid-section-footer {
    background-image: url(../../assets/img/footer-bg.jpg);
    display: flex;
    flex-grow: 1;
}

#logo-container {
    img {
        width: 70%;
        object-fit: cover;
    }
}

.column {
    display: flex;
    flex-direction: column;
    color: grey;
    padding: 15px;
    width: calc(100% / 3);

    .title {
        color: white;
    }
}
</style>