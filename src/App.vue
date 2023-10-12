<script>
import axios from 'axios';
import Header from './components/Header.vue';
import Selector from './components/Selector.vue';
import CardContainer from './components/CardContainer.vue';
export default {
  name:"App",
  components:{
    Header,
    Selector,
    CardContainer
  }

}
</script>

<template>
  <Header />
  <selector />
  <CardContainer />
</template>


<style lang="scss">
@use './scss/main.scss';
</style>