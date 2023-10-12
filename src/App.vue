<script>
import axios from 'axios';
import Header from './components/Header.vue';
import Selector from './components/Selector.vue';
export default {
  name:"App",
  components:{
    Header,
    Selector
  }

}
</script>

<template>
  <Header />
  <selector />
</template>


<style lang="scss">
@use './scss/main.scss';
</style>