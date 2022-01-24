<template>
  <div>
     <div class="header-container">
      <div class="header-top">
        <img src="../assets/img/logo-sidearea-1.png" alt="">
        <ul>
          <li><a class="active" href="#">home</a></li>
          <li><a href="#">home</a></li>
          <li><a href="#">home</a></li>
          <li><a href="#">home</a></li>
          <li><a href="#">home</a></li>
          <li><a href="#">home</a></li>
          <li><a href="#">home</a></li>
        </ul>
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
      // height: 40px;
      padding: 1em;
      width: 100%;
      background-color: white;
      display: flex;
      justify-content: space-between;

      img {
        width: 5%;
      }

      ul {
        list-style: none;
        display: flex;

        li {
          a {
            color: black;
            text-decoration: none;
            text-transform: uppercase;
            font-size: 0.6em;
            font-weight: bold;
            margin-right: 2em;
          }

          a:hover,
          a:active,
          .active {
            border-bottom: 3px solid #f5d8ca;
          }
        }
      }
    }
  }
</style>