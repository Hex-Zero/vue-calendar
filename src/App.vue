<template>
  <img alt="Vue logo" ref="logo" src="./assets/logo.png">
  <button @click="handleClick">show</button>
</template>

<script>
export default {
  name: 'App',
  data(){
    return{
      greeting: "OI"
    }
  },
  methods:{
  handleClick(){
    console.log(this.$refs.logo);
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
</style>
