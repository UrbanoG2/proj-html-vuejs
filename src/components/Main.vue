<template>
  <div>
      <div class="main-container">
            <div class="images-container">
                big-images
            </div>

            <div class="working-process-container">
                <div class="working-process-contained">
                    working-process
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
export default {
    name:"Main"
}
</script>

<style lang="scss" scoped>
    .main-container {
        width: 100%;
        .images-container {
            width:100%;
            height: 800px; 
            background-color: brown;   
        }

        .working-process-container {
            width: 100%;
            height: 400px;
            background-color: rgb(20, 214, 221);

            .working-process-contained {
                width: 60%;
                height: 100%;
                margin: 0 auto;
                background-color: chartreuse;
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