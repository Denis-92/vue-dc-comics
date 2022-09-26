<template>
  <div id="app">
    <pageHeaderVue />
    <pageMainVue />
    <pageFooterVue />
  </div>
</template>


<script>
import pageHeaderVue from './components/pageHeader.vue';
import pageMainVue from './components/pageMain.vue';
import pageFooterVue from './components/pageFooter.vue';

export default {
  name: 'App',
  components: {
    pageHeaderVue,
    pageMainVue,
    pageFooterVue,
  }
}
</script>


<style lang="scss">
@import './style/generics.scss';

.section-container {
  max-width: 1200px;
  margin: 0 auto;
}
</style>
