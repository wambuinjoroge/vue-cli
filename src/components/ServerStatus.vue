<template>
    <div>
        <p>Server status: {{ status }}</p>
        <hr>
        <button @click="changeStatus">Change Status</button>
    </div>

</template>

<script>
    export default {
        data: function () {
            return{
                status:"Critical"
            }
        },
        methods:{
            changeStatus(){
                this.status = "Stable"
            }
        }
    }
</script>

<style>

</style>