<template>
    <header>
        <img :src="resortImage" alt="Resort Image">
    </header>
</template>

<script>
    import resortImage from '@/assets/bresort.jpg';
    
    export default {
        name: 'TopHeader',
        data() {
            return {
                resortImage
            };
        }
    }
</script>

<style>
    img {
        width: 100%;
        display: block;
    }
</style>