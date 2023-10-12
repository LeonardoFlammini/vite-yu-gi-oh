<script>
export default {
  name: "Header"
}
</script>

<template>
  <header class="d-flex align-items-center ">
    <div class="logo">
      <img src="/logo.png" alt="logo">
    </div>
    <h1 class="ms-5">Yu-Gi-Oh!</h1>
    <select class="form-select" name="type" id="type">
      <option value="0">Seleziona un tipo</option>
    </select>
  </header>
</template>



<style scoped lang="scss">

header{
  background-color: white;
  width: 100%;
  height: 90px;
  .logo{
    width: 150px;
  }
  h1{
    font-weight: bold;
  }
  #type{
    width: 200px;
    margin-left: 150px;
  }
}
</style>