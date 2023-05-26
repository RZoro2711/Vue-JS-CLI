<template>
  <span>
    <p>Hello Vue JS</p>
    <div v-if="showModal">
      <Modal :theme="theme" @close="showModal = false">
        <h2>{{ header }}</h2>
        <p>{{ body }}</p>
      </Modal>
    </div>
    <button @click="showModal = true">Show Modal</button>
  </span>
</template>

<script>
import Modal from './components/ModalComponent.vue';
export default {
  data() {
    return {
      header: "Login Success",
      body: "Welcom Back!",
      theme: "success",
      showModal: false,
    }
  },
  components: { Modal }
}
</script>

<style scoped>
p {
  color: blue;
}
</style>