
<script>
export default {
  name:"Card",
  props:{
    name: String,
    archetype: String,
    image: String
  }

}
</script>

<template>
  <div class="col">
    <div class="card">
      <img :src="image" class="card-img-top" :alt="name">
      <div class="card-body text-center">
        <h5 class="card-title name">{{name}}</h5>
        <p class="card-text archetype">{{archetype}}</p>
      </div>
    </div>
  </div>
</template>


<style scoped lang="scss">

</style>