<template>
  <div>
      <div class="footer-container">
          <div class="footer-contained">
                <div class="footer-square">
                    <div class="inside-footer-box">
                        <img src="../assets/img/logo-sidearea-1.png" alt="">
                        <h5>Let's Get Creative</h5>
                    </div>
                </div>
                <div class="footer-square">
                    <div class="inside-footer-box">
                        <h5>maree.qode@gmail.com</h5>
                        <h5>+44645 321 789</h5>
                    </div>
                </div>
                <div class="footer-square">
                    <div class="inside-footer-box">
                        <h5>Avenue d'Auderghem 10</h5>
                        <h5>1040 Bruxelles, Belgium</h5>
                    </div>
                </div>
                <div class="footer-square">
                    <div class="inside-footer-box">
                        <h5>Stay in touch with us</h5>
                        <div class="socials">
                            <a href=""><font-awesome-icon :icon="['fab', 'twitter']" /></a>
                            <a href=""><font-awesome-icon :icon="['fab', 'pinterest-p']" /></a>
                            <a href=""><font-awesome-icon :icon="['fab', 'facebook-f']" /></a>
                            <a href=""><font-awesome-icon :icon="['fab', 'linkedin-in']" /></a>

                        </div>
                    </div>
                </div>
          </div>
      </div>
  </div>
</template>



<script>

// import { library } from '@fortawesome/fontawesome-svg-core'
// import { faUserSecret } from '@fortawesome/free-solid-svg-icons'
// import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome'


// library.add(faUserSecret)

import { library } from '@fortawesome/fontawesome-svg-core'
import { faTwitter } from '@fortawesome/free-brands-svg-icons'
import { faPinterestP } from '@fortawesome/free-brands-svg-icons'
import { faFacebookF } from '@fortawesome/free-brands-svg-icons'
import { faLinkedinIn } from '@fortawesome/free-brands-svg-icons'
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome'

library.add(faTwitter)
library.add(faPinterestP)
library.add(faFacebookF)
library.add(faLinkedinIn)

export default {
    name:"Footer",
    components: {
        FontAwesomeIcon
    }
}
</script>

<style lang="scss" scoped>
    .footer-container {
        width: 100%;
        background-color: #c0e1cf;
        margin-top: 3em;
        margin-bottom: 3em;
        padding: 3em 0;

        .footer-contained {
            width: 60%;
            height: 100%;
            margin: 0 auto;
            display: flex;

            .footer-square {
                width: calc(100% / 4);
                height: 100%;
                margin: 10px;
                display: flex;
                align-items: center;
                justify-content: center;

                .inside-footer-box {
                    h5 {
                        font-weight: normal;
                        margin: 1em 0;
                    }

                    img {
                        width: 80%;
                    }

                    .socials {
                        display: flex;
                        justify-content: space-between;
                        
                        a {
                            color: black;
                        }
                    }
                }
            }
        }
    }
</style>