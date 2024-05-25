<template>
    <div class="backdrop" v-if="isvisible">
        <div class="modal" :class="{sale: theme === 'sale'}">
            <div class="x-factor" @click="change"> x</div>
            <iframe src="https://www.youtube.com/watch?v=hd_MKrvcmFQ" frameborder="0" width="100%" height="400px"></iframe>
            
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
        position: fixed;
        margin-top: -60px;
        justify-content: center;
        z-index: 1;
        left: 0;
        width: 100%; /* Full width */
        height: 100%; /* Full height */
        display: flex;
        justify-content: center;

    }
    .modal{
        color: black;
        font-family: Arial, Helvetica, sans-serif;
        font-size: 20px;
        background-color: white;
        width: 550px;
        height: 450px;
        border: black solid 2px;
        margin-top: 200px;
        padding: 0 70px;
    }
    .x-factor{
        margin-right: 20px;
        float: right;
        font-weight: 700;
        cursor: pointer;
    }
    .modal p{
        color: aliceblue;
    }

    .modal.sale{
        background-color: rgb(0, 179, 255);
        
    }
</style>

