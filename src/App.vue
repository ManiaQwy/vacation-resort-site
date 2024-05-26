<template>

  <div id="container">
    <MyModal />
    <TopHeader />
    <NavIgation/>
    <SecTion />
    <DownFooter />
  </div>

  <!-- prop export -->



</template>
<script>
import MyModal from './components/MyModal.vue'
import TopHeader from './components/TopHeader.vue'
import SecTion from './components/SecTion.vue'
import NavIgation from './components/NavIgation.vue'
import DownFooter from './components/DownFooter.vue'

export default {
  name: 'App',
  components: { MyModal,TopHeader,SecTion,DownFooter,NavIgation },
  data(){
    return{
      title: "we are doing text!?!?!",
      text: "bonus text to learn binding with props"
    }
  },
  methods:{
    // deviousbutton(){
    //   console.log(this.$refs.name);
    //   this.$refs.name.classList.add('active');
    //   this.$refs.name.focus()
    // using refs to give an object a class

    }
  }

</script>

<style>
#container{
  max-width: 1000px;
  height: 2000px;
  background-color: darkcyan;
  margin:0 auto;
  box-sizing: border-box;
  overflow: hidden;
}
#app {
  font-family: Helvetica, Arial, sans-serif;
  text-align: center;
  background-color: #ddb;
  box-sizing: border-box;
  
}
p{
  font-size: 50px;
  font-weight: 700;
}


</style>
