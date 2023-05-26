<template>
  <div class="backdrop">
    <div class="modal" :class='{success:theme=="success",danger:theme=="delete"}'>
        <h2>{{ header }}</h2>
        <p>{{ body }}</p>
    </div>
  </div>
</template>

<script>
export default {
props : ['header', 'body', "theme"]
}
</script>

<style scoped>
    .backdrop{
        width: 100%;
        height: 100%;
        position: fixed;
        top: 0;
        left: 0;
        background: rgba(0, 0, 0, 0.5);
    }
    .modal{
        width: 400px;
        height: 50px;
        margin: 100px auto;
        background: white;
        border-radius: 10px;
        padding: 50px;
    }
    h2{
      margin-bottom: 10px;
    }
    .success{
      background: green;
      color: white;
    }
    .danger{
      background: red;
      color: white;
    }
</style>