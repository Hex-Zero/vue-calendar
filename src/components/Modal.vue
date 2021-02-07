<template>
  <div class="backdrop">
    <div class="modal">
      <p>{{ greeting }}</p>
    </div>
  </div>
</template>

<script>
export default {
  props: ["greeting"],
};
</script>

<style scoped>
.modal {
  width: 400px;
  padding: 20px;
  margin: 100px auto;
  background: white;
}
.backdrop {
  top: 0;
  position: fixed;
  background: #fdfdfd62;
  width: 100%;
  height: 100%;
}
</style>
