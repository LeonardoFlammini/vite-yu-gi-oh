
<script>
export default {
  name: "Selector"
}
</script>

<template>
  <div class="container bar-container">
    <div class="bar ">
      <select class="form-select" name="type" id="type">
        <option value="0">Seleziona un tipo</option>
      </select>
    </div>
  </div>
</template>


<style scoped lang="scss">
@use "../scss/partials/vars.scss" as *;
.bar-container{
  background-color: $container-bg-color;
  .bar{
  width: 100%;
  
  padding: $padding-container;
  #type{
    width: 200px;
  }
}
}
  
</style>