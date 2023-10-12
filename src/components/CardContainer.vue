<script>
import { store } from '../data/store.js';
import Card from './Card.vue';
export default {
  name: "CardContainer",
  components:{
    Card
  },
  data(){
    return{
      store
    }
  }
}
</script>

<template>
  <div class="container card-container">
    <div class="row row-cols-4 row-gap-3 align-items-stretch">
      <Card
      v-for="card in store.cardList"
      :key="card.id"
      :name="card.name"
      :archetype="card.archetype"
      :image="card.card_images[0].image_url"
      />
      
    </div>
  </div>
</template>



<style scoped lang="scss">
@use "../scss/partials/vars.scss" as *;
.card-container{
  // display: flex;
  // flex-wrap: wrap;
  min-height: 1000px;
  background-color: $container-bg-color;
  padding: $padding-container;
}
</style>