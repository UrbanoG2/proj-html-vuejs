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
        <div class="slider-container active">
            <font-awesome-icon @click ="getActive" id="angle-left" icon="angle-left" />
            <div class="slider-contained">


              <div class="slider-contained-left">
                <div class="text-container">
                  <h1>Devotion that never <span>ends</span></h1>
                  <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Suscipit dolores blanditiis ad corporis quis earum voluptate saepe </p>
                  <button><a href="#">Read more</a></button>
                </div>
              </div>

              <div class="slider-contained-right">
                <img src="../assets/img/h-2-slider-img-15.png" class="main-images" alt="">
                <img src="../assets/img/h-2-slider-img-16.png" class="main-images" alt="">
                <img src="../assets/img/short-slider-rev-1-img-2.png" id="petal" alt="">
                <img src="../assets/img/short-slider-rev-1-img-6.png" id="petal-2" alt="">
                <img src="../assets/img/short-slider-rev-1-img-7.png" id="purple-leaf" alt="">
                <img src="../assets/img/short-slider-rev-1-img-8.png" id="white-leaf" alt="">
                <img src="../assets/img/short-slider-rev-1-img-10.png" id="pink-leaf" alt="">
                <img src="../assets/img/h-2-slider-img-17.png" id="flowers" alt="">

              </div>
            </div>
            <font-awesome-icon @click ="getActive" id="angle-right" icon="angle-right" />


        </div>

        <div class="slider-container display-none">
            <font-awesome-icon @click ="getActive" id="angle-left" icon="angle-left" />
            <div class="slider-contained">


              <div class="slider-contained-left">
                <div class="text-container">
                  <h1>Hope this thing <span>works</span></h1>
                  <p>Second paragraph: walking through my mind while i write thing </p>
                  <button><a href="#">You interested?</a></button>
                </div>
              </div>

              <div class="slider-contained-right">
                <img src="../assets/img/h-2-slider-img-11.png" class="main-image-2" alt="">
                <img src="../assets/img/short-slider-rev-1-img-7.png" id="purple-leaf" alt="">
                <img src="../assets/img/short-slider-rev-1-img-8.png" id="white-leaf" alt="">
                <img src="../assets/img/h-2-slider-img-17.png" id="flowers" alt="">

              </div>
            </div>
            <font-awesome-icon @click ="getActive" id="angle-right" icon="angle-right" />


        </div>
      </div>
      
  </div>
  </div>
</template>

<script>

import { library } from '@fortawesome/fontawesome-svg-core'
import { faAngleLeft } from '@fortawesome/free-solid-svg-icons'
import { faAngleRight } from '@fortawesome/free-solid-svg-icons'
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome'


library.add(faAngleLeft)
library.add(faAngleRight)



export default {
    name:"Header",
    components:{
      FontAwesomeIcon
    },
    data () {
      return {
        // counter: null,
        // sliderImages: []
      }
    },


    methods: {

      getActive() {
        let element = document.querySelectorAll(".slider-container");
        console.log(element);

        for (let i = 0; i < element.length; i++) {
          const singleElement = element[i];
          console.log(singleElement);

          if (singleElement.classList.contains("active")) {
          singleElement.classList.remove("active");
          singleElement.classList.add("display-none")
        } else if (singleElement.classList.contains("display-none")) {
          singleElement.classList.remove("display-none");
          singleElement.classList.add("active")
        }

        }
      }
    },

}
</script>

<style lang="scss" scoped>
  .header-container {
    width: 100%;
    height: 450px;

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

    .header-bottom {
      width: 100%;
      margin: 0 auto;
      height: calc(100% - 50px);

      .slider-container {
        width: 100%;
        height: 100% ;
        position: relative;

        #angle-left {
          position: absolute;
          top: 50%;
          left: 2%;
          background-color: #f3d0c7;
          border-radius: 50%;
          height: 20px;
          width: 20px;
          color: white;
        }

         #angle-right {
          position: absolute;
          top: 50%;
          right: 2%;
          background-color: #f3d0c7;
          border-radius: 50%;
          height: 20px;
          width: 20px;
          color: white;
        }

        #angle-left:hover,
        #angle-right:hover {
          cursor: pointer;
        }
        
        .slider-contained {
          width: 80%;
          height: 100%;
          margin: 0 auto;
          display: flex;

          .slider-contained-left {
            height: 100%;
            width: 50%;
            display: flex;
            align-items: center;
            justify-content: flex-end;

            .text-container {
              width: 70%;

              h1 {
                font-weight: normal;
                font-size: 4em;

                span {
                  font-weight: bold;
                  font-style: oblique;
                }
              }

              p{
                color: #a6a6a6;
                margin-top: 1em
              }

              button {
                background-color: white;
                padding: 0.7em 1.7em;
                margin-top: 1.5em;
                border: 2px solid #e1c0b0;
                a {
                  text-transform: uppercase;
                  color: black;
                  text-decoration: none;
                  font-size: 0.7em;
                  font-weight: bold;
                }
              }

              button:hover {
                background-color:#e1c0b0;
              }

              button:hover a {
                color: white;
              }
            }
          }

          .slider-contained-right {
            height: 100%;
            width: 50%;
            display: flex;
            justify-content: center;
            align-items: flex-end;
            position: relative;

            .main-images {
              width: 40%;
              height: 80%;
            }

            .main-image-2 {
              width: 100%;
              height: 100%;
            }

            #petal {
              position: absolute;
              top: 0;
              left: 10%;
            }

            #petal-2 {
              position: absolute;
              top: 30%;
              right: 10%;
            }

            #purple-leaf {
              transform: scaleX(-1);
              position: absolute;
              top: 0;
              right: 15%;
            }

            #white-leaf {
              transform: scaleX(-1);
              position: absolute;
              bottom: 0;
              left: 5%;
            }

            #pink-leaf {
              transform: scaleX(-1);
              position: absolute;
              bottom: 35%;
              left: 0;
            }

            #flowers {
              position: absolute;
              bottom: 0;
              right: 0;
            }
          }
        }
      }

      .display-none {
        display: none;
      }

      .active {
        display: block;
      }
    }
  }
</style>