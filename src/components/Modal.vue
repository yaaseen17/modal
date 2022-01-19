<template>
  <div class="backdrop" @click.self="closeModal">
    <div class="modal">
      <h1>hoyah</h1>
      <p>modal content</p>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    closeModal() {
      this.$emit("close");
    },
  },
};
</script>

<style scoped>
.modal {
  width: 400px;
  padding: 20px;
  margin: 100px auto;
  background: rgb(0, 0, 0);
  border-radius: 10px;
}
.backdrop {
  top: 0;
  position: fixed;
  background: transparent;
  width: 100%;
  height: 100%;
}
h1 {
  color: rgb(92, 255, 71);
}
</style>
