<template>
  <div>
      <div class="main-container">
            <div class="images-container">
                <div class="images">
                    <img src="../assets/img/h-2-port-img-1.jpg" alt="">
                    <img src="../assets/img/h-2-port-img-2.jpg" alt="">
                    <img src="../assets/img/h-2-port-img-3.jpg" alt="">
                    <img src="../assets/img/h-2-port-img-4.jpg" alt="">
                    <img src="../assets/img/h-2-port-img-5.jpg" alt="">
                    <img src="../assets/img/h-2-port-img-6.jpg" alt="">
                </div>
            </div>

            <div class="working-process-container">
                <div class="working-process-contained">
                    <h1>Working <span>process</span></h1>
                    <div class="process">
                        <div class="process-thumb">
                            <!-- <img src="../assets/svg/svg-8.svg" alt="">  -->

                            <font-awesome-icon style="color:lightblue" class="icon" icon="lightbulb" />
                            <div class="text-container">
                                <div class="title">
                                    First theres an idea
                                </div>
                                <div class="para">
                                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Corrupti, a accusamus
                                </div>
                            </div>
                        </div>
                        <div class="process-thumb">
                            <!-- <img src="../assets/svg/svg-8.svg" alt="">  -->

                            <font-awesome-icon style="color:darkyellow" class="icon" icon="comment" />
                            <div class="text-container">
                                <div class="title">
                                    Then we talk about
                                </div>
                                <div class="para">
                                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Corrupti, a accusamus
                                </div>
                            </div>
                        </div>
                        <div class="process-thumb">
                            <!-- <img src="../assets/svg/svg-8.svg" alt="">  -->

                            <font-awesome-icon style="color:purple" class="icon" icon="cloud" />
                            <div class="text-container">
                                <div class="title">
                                    And we think about
                                </div>
                                <div class="para">
                                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Corrupti, a accusamus
                                </div>
                            </div>
                        </div>
                        <div class="process-thumb">
                            <!-- <img src="../assets/svg/svg-8.svg" alt="">  -->

                            <font-awesome-icon style="color:crimson" class="icon" icon="pencil-ruler" />
                            <div class="text-container">
                                <div class="title">
                                    So we draw along
                                </div>
                                <div class="para">
                                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Corrupti, a accusamus
                                </div>
                            </div>
                        </div>
                        
                    </div>
                </div>
            </div> 

            <div class="contact-us-container">
                <div class="contact-us-container-top">
                    <div class="contact-us-contained-top">
                        <h1>Want to work with us? Send us <span>a message!</span></h1>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Rerum fugit blanditiis nesciunt! At expedita illum Lorem ipsum dolor sit amet consectetur adipisicing elit. Impedit voluptatibus veritatis hic, cum voluptates nobis perspiciatis, aliquam nihil totam cumque fugiat, aspernatur doloribus ratione omnis quae modi sunt reprehenderit? Adipisci!</p>

                        <button><a href="#">contact</a></button>
                    </div>
                </div>

                <div class="contact-us-bottom">
                    <div class="image-container">
                        <img src="../assets/img/h-2-blog-img-1.jpg" alt="">
                        <h3>This way, loves: a detailed guide through new design </h3>
                        <h5>By Emily Fields</h5>
                    </div>
                    <div class="image-container">
                        <img src="../assets/img/h-2-blog-img-2.jpg" alt="">
                        <h3>I try to give people a different way of looking art </h3>
                        <h5>By Emily Fields</h5>
                    </div>
                    <div class="image-container">
                        <img src="../assets/img/h-2-blog-img-3.jpg" alt="">
                        <h3>Introduce Richard Laperrière of those amazing features </h3>
                        <h5>By Emily Fields</h5>
                    </div>
                </div>
                
            </div> 

      </div>
  </div>
</template>

<script>

import { library } from '@fortawesome/fontawesome-svg-core'
// import { faUserSecret } from '@fortawesome/free-solid-svg-icons'
import { faLightbulb } from '@fortawesome/free-solid-svg-icons'
import { faComment } from '@fortawesome/free-solid-svg-icons'
import { faCloud } from '@fortawesome/free-solid-svg-icons'
import { faPencilRuler } from '@fortawesome/free-solid-svg-icons'
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome'

// library.add(faUserSecret)
library.add(faComment)
library.add(faCloud)
library.add(faPencilRuler)
library.add(faLightbulb)




export default {
    name:"Main",

    components:{
        FontAwesomeIcon 
    },
    // data() {
    //    return {
    //         mainImages:[
    //         "h-2-port-img-1.jpg",
    //         "h-2-port-img-2.jpg",
    //         "h-2-port-img-3.jpg",
    //         "h-2-port-img-4.jpg",
    //         "h-2-port-img-5.jpg",
    //         "h-2-port-img-6.jpg",
    //     ]
    //    }
    // }
}
</script>

<style lang="scss" scoped>
    .main-container {
        width: 100%;
        .images-container {
            width:100%;
            .images{
                
                display: flex;
                flex-wrap: wrap;
                img {
                    width: calc(100% / 3);
                }
            }
        }

        .working-process-container {
            width: 100%;
            height: 400px;

            .working-process-contained {
                width: 60%;
                height: 100%;
                margin: 0 auto;
                margin-top: 3em;
                
                h1 {
                    text-align: center;
                    font-size: 3em;
                    font-weight: normal;
                    span {
                        font-weight: bold;
                        font-style: oblique;
                    }
                }


                .process {
                    width: 100%;
                    height: 100%;
                    background-image: url(../assets/svg/svg-3.svg);
                    background-repeat: no-repeat;
                    margin-top: 3em;
                    display: flex;

                    .process-thumb {
                        height: 74%;
                        width: calc(100% / 4);
                        display: flex;
                        flex-direction: column;
                        align-items: center;
                        margin: 0 0.8em;

                        .icon {
                            font-size: 8em;
                            padding: 0.2em;
                            margin-bottom: 0.2em;
                        }

                        .text-container {
                            
                            text-align: center;
                            
                            .title {
                                font-weight: bold;
                            }

                            .para {
                                color: #a6a6a6;
                                font-size: 0.8em;
                                margin-top: 0.8em;
                                width: 100%;
                            }
                        }
                        
                    }
                }
            }
        }

        .contact-us-container {
            width: 100%;
            height: 700px;

            .contact-us-container-top {
                width: 100%;
                height: 50%;
                background-color: #f3d0c7;


                .contact-us-contained-top {
                    height: 100%;
                    width: 60%;
                    margin: 0 auto;
                    display: flex;
                    flex-direction: column;
                    align-items: center;
                    justify-content: center;

                    h1 {
                        font-weight: normal;
                        text-align: center;
                        font-size: 3em;
                        margin-bottom: 0.5em;

                        span {
                            font-weight: bold;
                            font-style: oblique;
                        }
                    }

                    p {
                        color: #a6a6a6;
                        text-align: center;
                        margin-bottom: 0.5em;
                    }

                    button {
                        padding:1em 1.5em;
                        margin-top: 1em;
                        border: none;
                        width: 15%;
                        background-color: #d8f0e3;

                        a {
                            color: black;
                            text-transform: uppercase;
                            font-weight: bold;
                            font-size: 0.8em;
                            text-decoration: none;
                        }
                    }

                    button:hover {
                        // cursor: url('https://www.pixelliongroup.com/img/cursor.png'), auto;
                        background-color: #f5d8ca;
                    }

                    button:hover a{
                        color: white;
                    }
                }
            }

            .contact-us-bottom {
                height: 50%;
                width: 60%;
                margin: 0 auto;
                display: flex;
                margin-top: 3em;
                
                .image-container {
                    width: calc(100% / 3);
                    margin: 10px;
                    img {
                        width: 100%;
                    }
                    h3,
                    h5 {
                        margin-top: 0.5em;
                        font-weight: normal;

                    }

                    h5 {
                        font-style: oblique;
                    }
                }
            }

        }
    }
</style>