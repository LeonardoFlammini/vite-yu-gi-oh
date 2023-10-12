
<script>
export default {
  name: "Selector"
}
</script>

<template>
  <div class="container">
    <div class="bar ">
      <select class="form-select" name="type" id="type">
        <option value="0">Seleziona un tipo</option>
      </select>
    </div>
  </div>
</template>


<style scoped lang="scss">
.bar{
  // height: 50px;
  width: 100%;
  background-color: rgba($color: #000000, $alpha: .5);
  padding: 20px;
  #type{
    width: 200px;
  }
}
</style>