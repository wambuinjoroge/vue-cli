<template>
<h1>Hello World,"Server is: {{status}}"</h1>
</template>

<script>
// a component is a reusable piece of our instance,basically extends the vue instance
    export default {
       data:function () {
            return{
                status:"Stable"
            }
        },

    }

</script>

<style>

</style>