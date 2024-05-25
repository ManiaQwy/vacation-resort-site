<template>
    <div class="backdrop" v-if="isvisible">
        <div class="modal" :class="{sale: theme === 'sale'}">
            <div class="x-factor" @click="change"> x</div>
            <p>Modal or smth idk in the middle of the tutorial</p>
            
        </div>
    </div>
    <p>{{ header }}</p>
    <p>{{ text }}</p>
</template>
<script>
    export default{
        props: ["header", "text", "theme"],   //prop export
        name: 'MyModal',
        data(){
            return {
                isvisible: true
            }
        },
        methods: {
            change(){
                this.isvisible = false
                
            }
        }
    }
</script>
<!-- or scoped -->
<style>  
    .backdrop{
        background-color: rgba(0, 0, 0, 0.484);
        width: 100%;
        height: 1500px;
        position: absolute;
        margin-top: -60px;
        display: flex;
        justify-content: center;
    }
    .modal{
        color: black;
        font-family: Arial, Helvetica, sans-serif;
        font-size: 20px;
        background-color: white;
        width: 450px;
        height: 350px;
        border: black solid 2px;
        margin-top: 200px;
        padding: 0 70px;
    }
    .x-factor{
        margin-right: 20px;
        float: right;
        font-weight: 700;
        
    }
    .modal p{
        color: aliceblue;
    }

    .modal.sale{
        background-color: rgb(9, 180, 115);
        
    }
</style>

