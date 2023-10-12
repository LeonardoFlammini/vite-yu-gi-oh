<script>
import axios from 'axios';
import { store } from './data/store';
import Header from './components/Header.vue';
import Selector from './components/Selector.vue';
import CardContainer from './components/CardContainer.vue';
export default {
  name:"App",
  components:{
    Header,
    Selector,
    CardContainer
  },
  data(){
    return{
      store
    }
  },
  methods:{
    getApi(){
      axios.get(store.apiUrl)
        .then( res =>{
          store.cardList = res.data.data;
          
        })
        .catch(err => {
          console.log(err);
        })

    }
  },
  mounted(){
    this.getApi();
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