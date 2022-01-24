<template>
  <div>
      <div class="footer-container">
          <div class="footer-contained">
              footer
          </div>
      </div>
  </div>
</template>

<script>
export default {
    name:"Footer"
}
</script>

<style lang="scss" scoped>
    .footer-container {
        width: 100%;
        height: 130px;
        background-color: darkcyan;

        .footer-contained {
            width: 60%;
            height: 100%;
            margin: 0 auto;
            background-color: darkgreen;
        }
    }
</style>