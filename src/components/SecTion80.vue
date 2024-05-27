<template>
    <section>
        <article>
            <h1>STRONA RESORT WAKACYJNY</h1>
            <p>
                <img class="left" alt="gosc" :src="SigmaBale"> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Fusce volutpat efficitur nisi a fermentum. Integer aliquam ultrices neque sit amet rhoncus. Aenean vestibulum efficitur dignissim. Phasellus a augue condimentum, luctus tortor nec, venenatis neque. Aliquam tempus diam leo, at tristique neque pharetra eleifend. Vivamus vitae elit at nibh congue ultrices.
            </p>
            <p>
                Vivamus vitae elit at nibh congue ultrices. Donec purus massa, rutrum a fringilla eget, ullamcorper vel eros. Aliquam vitae ex velit
            </p>
            <p>
                Etiam mauris leo, placerat quis diam vitae, fringilla bibendum tortor. Praesent vel elit nec nunc egestas mollis. Aenean mattis enim id est laoreet, eu commodo diam accumsan.
            </p>
            <p>
                Curabitur nisl diam, auctor nec dolor pulvinar, imperdiet ultricies risus. Nulla augue nisi, pulvinar vitae nibh et, ullamcorper dictum nisi. Fusce in commodo nisl.
            </p>
        </article>
        <iframe width="1000" height="564" src="https://www.youtube.com/embed/watch?v=SuEkOAayWZo" frameborder="0" title="Youtube Video"></iframe>
    </section>
</template>
<script>
    import SigmaBale from '@/assets/christian-bale-w-american-psycho.jpg';
    
    export default {
        name: 'SecTion80',
        data() {
            return {
                SigmaBale
            };
        }
    }
</script>
<style>
    section{
        background-color: white
    }
    article{
        margin-top: 30px;
        margin-bottom: 20px;
    }
    article h1{
        font-size: 30px;
        margin: 0px 10% 50px 10%;
        padding-top: 30px;
        background-color: white;
        text-align: center;
        border-bottom: solid crimson 2px;
        padding-bottom: 15px;
        font-weight: 700;
    }
    article p{
        text-align: justify;
        padding: 5px 20px;
        line-height: 1.3;
    }
    img.left{
        float: left;
        padding: 0 10px 10px 10px;
        width: 20%;
        border-radius:30px ;
    }
    iframe{
        width: 100%;
    }
</style>