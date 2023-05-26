<template>
  <p>Hello Vue JS</p>
  <Modal/>
</template>

<script>
import Modal from './components/ModalComponent.vue';
export default {
  components: { Modal }
}
</script>

<style scoped>
p {
  color: blue;
}
</style>