<template>
<div>

   <!--<app-servers></app-servers>-->

    <!--<button @click="selectedComponent = 'app-quote'">-->
        <!--Quote-->
    <!--</button>-->
    <!--<button @click="selectedComponent = 'app-author'">-->
        <!--Author-->
    <!--</button>-->
    <!--<button @click="selectedComponent = 'app-new'">-->
        <!--New Quote-->
    <!--</button>-->
    <!--<p>{{ selectedComponent }}</p>-->
    <!--<keep-alive>-->
        <!--<component :is="selectedComponent"></component>-->
    <!--</keep-alive>-->
   <!--<app-quote>-->
       <!--<h1 slot="title">Hello World</h1>-->
       <!--<h1 slot="content">You better be ready!!</h1>-->
   <!--</app-quote>-->

    <app-landing></app-landing>
    <app-card></app-card>
    <app-house v-for="house in 3" class="col-xs-3"></app-house>

</div>

</template>

<script>
// a component is a reusable piece of our instance,basically extends the vue instance
import Quote from "./components/Quote";
import Author from "./components/Author";
import New from "./components/New";
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
        "app-quote":Quote,
        "app-author":Author,
        "app-new":New,
        "app-house":House,
        "app-landing":Landing,
        "app-card":Card,
    },
}
</script>

<style>

</style>