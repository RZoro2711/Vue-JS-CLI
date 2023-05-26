<template>
  <div class="backdrop">
    <div class="modal">
        <p>Modal Component</p>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>
    .backdrop{
        width: 100%;
        height: 100%;
        position: fixed;
        top: 0;
        left: 0;
        background: rgba(0, 0, 0, 0.5);
    }
    .modal{
        width: 200px;
        height: 100px;
        margin: 100px auto;
        background: white;
        border-radius: 10px;
        padding: 100px;
        text-align: center;
    }
</style>