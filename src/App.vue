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
    <div v-if="showModalTwo">
      <Modal :theme="theme" @close="showModalTwo = false">
        <h2>{{ del_header }}</h2>
        <p>{{ del_body }}</p>
      </Modal>
    </div>
    <button @click="showModalTwo = true">Log out Modal</button>
  </span>
</template>

<script>
import Modal from './components/ModalComponent.vue';
export default {
  data() {
    return {
      header: "Login Success",
      body: "Welcom Back!",
      del_header : "Wanna Delete",
      del_body : "Successful",
      theme: "success",
      showModal: false,
      showModalTwo: false,
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