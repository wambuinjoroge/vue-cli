<template>
    <div>
    <h2>The Author</h2>
        <button @click="increaseCounter">Click to increase</button>
        <p>{{ counter }}</p>
    </div>

</template>

<script>
export default {
    data:function () {
        return{
          counter:0
        };
    },
    methods:{
        increaseCounter(){
            this.counter++;
        }
    },
    destroyed(){
        console.log("Destroyed")
    },
    deactivated(){
        console.log("Deactivated")
    },
    activated(){
        console.log("Activated")
    }
}
</script>

<style>

</style>