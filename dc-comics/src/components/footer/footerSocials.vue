<template>
    <div>
        <div id="socials-container">
            <div id="sign-up">SIGN-UP NOW!</div>
            <div class="social-logos">
                <div id="follow-us">FOLLOW US</div>
                <div><img src="@/assets/img/footer-facebook.png" alt="facebook logo"></div>
                <div><img src="@/assets/img/footer-twitter.png" alt="twitter logo"></div>
                <div><img src="@/assets/img/footer-youtube.png" alt="youtube logo"></div>
                <div><img src="@/assets/img/footer-pinterest.png" alt="pinterest logo"></div>
                <div><img src="@/assets/img/footer-periscope.png" alt="periscope logo"></div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "footerSocials"
}
</script>

<style lang="scss" scoped>
#socials-container {
    background-color: #333;
    height: 100px;
    width: 100%;
    display: flex;
    justify-content: space-between;
    padding: 30px;
}

#sign-up {
    color: white;
    padding: 10px;
    border: 2px solid blue;
    font-size: 1.1rem;
}

#follow-us {
    color: lightseagreen;
    font-weight: 700;
}

.social-logos {
    display: flex;
    align-items: center;

    * {
        padding: 5px;
    }
}
</style>