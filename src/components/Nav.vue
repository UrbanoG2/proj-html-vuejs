<template>
  <div>
      <ul>
          <li v-for="(item, index) in navLi"
              :key="index" 
          ><a :class="classLi" :href="url">{{ name }}</a></li>
          <!-- <li><a href="#">pages</a></li>
          <li><a href="#main-container">portfolio</a></li>
          <li><a href="#blog">blog</a></li>
          <li><a href="#">shop</a></li>
          <li><a href="#">elements</a></li> -->
          <li><a href="#"><img class="menu-icon" src="../assets/svg/svg-1.svg" alt=""></a></li>
        </ul>
  </div>
</template>

<script>
export default {
    name:"Nav",
    props:{
        classLi:String,
        url:String,
        name:String,
    },
}
</script>

<style lang="scss" scoped>
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
            margin-right: 3em;
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
</style>