<template>
<div style="font-family: Verdana, Geneva, sans-serif">

    <app-landing></app-landing>
    <!--<app-card></app-card>-->

    <div class="container">
        <h3>Homes for you</h3>
        <div class="row">
            <app-house v-for="house in 4" class="col-lg-3"></app-house>
        </div>
    </div>



</div>

</template>

<script>
// a component is a reusable piece of our instance,basically extends the vue instance

import House from "./components/houses/house";
import Landing from "./components/houses/landing";
import Card from "./components/houses/card";

export default {
    data:function () {
        return{
            selectedComponent: "app-quote"
        }
    },
    components:{
        "app-house":House,
        "app-landing":Landing,
        "app-card":Card,
    },
}
</script>

<style scoped>
    div.container{
        margin-top: 20px;
    }
    h3{
        font-weight: 700;
        margin-bottom: 0;
    }
</style>