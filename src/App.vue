<template>
  <p>Hello Vue JS</p>
  <Modal :header="header" :body="body" :theme="theme"></Modal>
</template>

<script>
import Modal from './components/ModalComponent.vue';
export default {
  data() {
    return {
      header: "Login Success",
      body: "Welcom Back!",
      theme: "success",
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