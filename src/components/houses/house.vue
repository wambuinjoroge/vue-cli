<template>
    <div class="container">
       <!--<div class="row">-->
           <!--<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQP3Wm95bNxJEeTMjVSBbgNBlOZD8OsX4LMu5q0R_dVkI8eFQU1" style="border-radius: 05px;" >-->
           <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQfmSzTes_aH7-4iiMXFTZCq7kLIcbj7i43_B0aOXGOz6UC9n55" style="border-radius: 05px;">

        <div class="img-content">
            <button @click="nextImage" class="btn btn-secondary btn-sm">1</button>
            <button class="btn btn-secondary btn-sm">2</button>
            <button class="btn btn-secondary btn-sm">3</button>

            <a href="" style="text-decoration: none;">
                <p class="house-name">A spacious Vue House</p>
                <p class="house-desc">Lorem Ipsum is simply dummy text of the printing and typesetting industry</p>
            </a>
        </div>

       <!--</div>-->
    </div>
</template>

<script>
    export default {

    }
</script>

<style scoped>
    a p.house-name{
        color: darkred;
        font-weight: bold;
        margin-bottom: 0;
    }
    a p.house-desc{
        color: darkred;
        font-weight: lighter;
    }
    img {
        /*margin-top: 5px;*/
        margin-bottom: 5px;
        max-width: 100%;
        height: auto;
    }
    .img-content{
        margin-top: 5px;
    }
</style>