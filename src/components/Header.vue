<script>
export default {
  name: "Header"
}
</script>

<template>
  <header>
    <div class="logo d-flex align-items-center justify-content-center ">
      <img src="/logo.png" alt="logo">
      <div>ciao</div>
    </div>
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
}
</style>