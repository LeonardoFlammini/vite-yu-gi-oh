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
}
</style>