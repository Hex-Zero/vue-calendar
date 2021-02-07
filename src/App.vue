<template>
  <img alt="Vue logo" ref="logo" src="./assets/logo.png" />
  <button @click="handleClick">show</button>
  <Modal greeting="Hello" v-if="showModal" />
</template>

<script>
import Modal from "./components/Modal.vue";
export default {
  name: "App",
  components: {
    Modal,
  },
  data() {
    return {
      greeting: "Hi",
      showModal: false,
    };
  },
  methods: {
    handleClick() {
      this.showModal = true;
    },
  },
};
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
