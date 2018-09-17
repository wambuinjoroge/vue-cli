<template>
    <div class="container">
       <div class="row">
               <!--<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQP3Wm95bNxJEeTMjVSBbgNBlOZD8OsX4LMu5q0R_dVkI8eFQU1" style="border-radius: 05px;" >-->
               <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQfmSzTes_aH7-4iiMXFTZCq7kLIcbj7i43_B0aOXGOz6UC9n55" style="border-radius: 05px;" width="460" height="345">

                 <button @click="nextImage">1</button>
                 <button>2</button>
                 <button>3</button>

                 <a href="#" style="text-decoration: none;">
                     <p class="house-name">A spacious Vue House</p>
                 </a>
       </div>
    </div>
</template>

<script>
    export default {
        data(){
          return {
              image : ""
          }
        },
        methods:{
            nextImage(){
                this.image = "the image you want"
            }
        }
    }
</script>

<style scoped>
    a p{
        color: darkred;
    },
    img {
        margin-top: 5px;
        max-width: 100%;
        height: auto;
    }
</style>