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

                            <font-awesome-icon id="icon" icon="user-secret" />
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

                            <font-awesome-icon id="icon" icon="user-secret" />
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

                            <font-awesome-icon id="icon" icon="user-secret" />
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

                            <font-awesome-icon id="icon" icon="user-secret" />
                            <div class="text-container">
                                <div class="title">
                                    First theres an idea
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
                <div class="contact-us-contained">
                    want to work with us?
                </div>
            </div> 

      </div>
  </div>
</template>

<script>

import { library } from '@fortawesome/fontawesome-svg-core'
import { faUserSecret } from '@fortawesome/free-solid-svg-icons'
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome'

library.add(faUserSecret)
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

                        #icon {
                            font-size: 9em;
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
            background-color: chocolate;

            .contact-us-contained {
                width: 60%;
                height: 100%;
                margin: 0 auto;
                background-color: crimson;
            }
        }
    }
</style>