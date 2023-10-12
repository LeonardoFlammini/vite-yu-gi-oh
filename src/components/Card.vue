
<script>
export default {
  name:"Card",
  props:{
    name: String,
    archetype: String,
    image: String
  },
  computed: {
    printArchetype(){
      if(this.archetype !== undefined){
        return this.archetype;
      }
      return "\"Not Archetyped\""
    }
  }

}
</script>

<template>
  <div class="col">
    <div class="card" style="height: 100%">
      <img :src="image" class="card-img-top" :alt="name">
      <div class="card-body text-center">
        <h5 class="card-title name">{{name}}</h5>
        <p class="card-text archetype">{{printArchetype}}</p>
      </div>
    </div>
  </div>
</template>


<style scoped lang="scss">
.archetype{
  text-decoration: underline;
}
</style>