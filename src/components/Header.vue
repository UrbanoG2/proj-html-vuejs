<template>
  <div>
     <div class="header-container">
      <div class="header-top">
        nav
      </div>

      <div class="header-bottom">
        slider
      </div>
      
  </div>
  </div>
</template>

<script>
export default {
    name:"Header"
}
</script>

<style lang="scss" scoped>
  .header-container {
    width: 100%;
    height: 400px;
    background-color: aqua;

    .header-top {
      height: 40px;
      width: 100%;
      background-color: blue;
    }
  }
</style>