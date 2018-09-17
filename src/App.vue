<template>
<div class="container">
    <h2>Get a house now!!!</h2>

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

    <app-house v-for="house in 12" class="col-xs-3"></app-house>
</div>

</template>

<script>
// a component is a reusable piece of our instance,basically extends the vue instance
import Quote from "./components/Quote";
import Author from "./components/Author";
import New from "./components/New";
import House from "./components/houses/house";

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
    },
}
</script>

<style scoped>
  h2{
      font-weight: bold;
  }
</style>