<template>

  <div id="container">
    <MyModal header="Random aah string moment" :text="text" theme="sale"/>
    <TopHeader />
  </div>
  <TopHeader />

  <!-- prop export -->



</template>
<script>
import MyModal from './components/MyModal.vue'
export default {
  name: 'App',
  components: { MyModal },
  data(){
    return{
      title: "we are doing text!?!?!",
      text: "bonus text to learn binding with props"
    }
  },
  methods:{
    deviousbutton(){
      console.log(this.$refs.name);
      this.$refs.name.classList.add('active');
      this.$refs.name.focus()
      // using refs to give an object a class

    }
  }
}
</script>

<style>
#container{
  width: 1000px;
  height: 2000px;
  background-color: rgb(231, 209, 96);
  margin:0 auto;
  box-sizing: border-box;
  overflow: hidden;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  text-align: center;
  background-color: rgb(0, 179, 255);
  box-sizing: border-box;
  
}
p{
  font-size: 50px;
  font-weight: 700;
}


</style>
