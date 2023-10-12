<script>
export default {
  name: "CardContainer"
}
</script>

<template>
  <div class="container card-container">

  </div>
</template>



<style scoped lang="scss">
@use "../scss/partials/vars.scss" as *;
.card-container{
  min-height: 1000px;
  background-color: $container-bg-color;
}
</style>