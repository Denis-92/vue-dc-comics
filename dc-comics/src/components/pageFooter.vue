<template>
    <div>
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

</style>