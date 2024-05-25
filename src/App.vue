<template>
  <MyModal header="Random aah string moment" :text="text" theme="sale"/>
  <!-- prop export -->
  <p>{{title}}</p>
  <input type="text" ref="name">
  <!-- refs -->
  <button @click="deviousbutton">make it RED</button>


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
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
p{
  font-size: 50px;
  font-weight: 700;
}

.active{
  background-color: red;
}
</style>
