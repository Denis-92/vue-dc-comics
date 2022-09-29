<template>
  <div id="app">
    <pageHeaderVue />
    <div id="jumbotron">
      <img src="@/assets/img/jumbotron.jpg" alt="Jumbotron">
      <div id="current-series">CURRENT SERIES</div>
    </div>
    <pageMainVue :cards="comics" />
    <pageFooterVue />
  </div>
</template>


<script>
import pageHeaderVue from './components/pageHeader.vue';
import pageMainVue from './components/pageMain.vue';
import pageFooterVue from './components/pageFooter.vue';
// import { comics } from '@/assets/data/dc-comics.js'
import comics from '@/assets/data/dc-comics.json'

export default {
  name: 'App',
  components: {
    pageHeaderVue,
    pageMainVue,
    pageFooterVue,
  },
  data() {
    return { comics }
  }
}
</script>


<style lang="scss">
@import './style/generics.scss';

.section-container {
  max-width: 1200px;
}

.margin-section {
  margin: 0 auto;
}

#app {
  display: flex;
  flex-direction: column;
  height: 100vh;
}

#jumbotron {
  height: 350px;

  img {
    width: 100%;
  }
}

#current-series {
  color: white;
  background-color: lightseagreen;
  position: absolute;
  padding: 5px 25px;
  font-size: 1.5rem;
  top: 61%;
  left: .6%;
}
</style>
