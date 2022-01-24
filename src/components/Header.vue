<template>
  <div>
     <div class="header-container">
      <div class="header-top">
        <img src="../assets/img/logo-sidearea-1.png" alt="">
        <ul>
          <li><a class="active" href="#">home</a></li>
          <li><a href="#">pages</a></li>
          <li><a href="#">portfolio</a></li>
          <li><a href="#">blog</a></li>
          <li><a href="#">shop</a></li>
          <li><a href="#">elements</a></li>
          <li><a href="#"><img class="menu-icon" src="../assets/svg/svg-1.svg" alt=""></a></li>
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
    name:"Header",
    data () {
      return {
        counter: null,
        sliderImages: []
      }
    },


    methods: {
      // prev: function () {
      //       this.counter -= 1;

      //       if (this.counter < 0) {
      //           this.counter = this.images.length - 1;
      //       }
      //   },

      //   next: function () {
      //       this.counter += 1;

      //       if (this.counter > this.images.length - 1) {
      //           this.counter = 0;
      //       }
      //   },

      //   changeOnClick: function (index) {
      //       console.log(index);
      //       this.counter = index;
      //   }
    },

    created() {
      this.images = [
        "h-2-slider-img-11.png",
        "h-2-slider-img-15.png",
        "h-2-slider-img-16.png"
      ],

      this.counter = 0;
    }
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

          .menu-icon {
            width: 18%;
          }
        }
      }
    }
  }
</style>