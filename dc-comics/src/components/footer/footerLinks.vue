<template>
    <div id="footer-links-container">

        <div class="column">
            <div>DC COMICS</div>
            <div>Characters</div>
            <div>Comics</div>
        </div>
        <div class="column">
            <div>DC</div>
            <div>Terms Of Use</div>
        </div>
        <div class="column">
            <div>SITES</div>
            <div>DC</div>
            <div>MAD Magazine</div>
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
    background-image: url(../../assets/img/footer-bg.jpg);
    display: flex;
    padding: 15px;
}

.column {
    display: flex;
    flex-direction: column;
    color: white;
    padding: 15px;
}
</style>