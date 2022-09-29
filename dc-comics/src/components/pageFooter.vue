<template>
    <div id="footer-container">
        <footerLinks />
        <footerSocials />
    </div>
</template>

<script>
import footerSocials from './footer/footerSocials.vue';
import footerLinks from './footer/footerLinks.vue';

export default {
    name: "pageFooter",
    components: {
        footerSocials,
        footerLinks,
    }
}
</script>

<style lang="scss" scoped>
#footer-container {
    display: flex;
    flex-direction: column;
    flex-grow: 1;
}
</style>