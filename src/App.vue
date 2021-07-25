<template>
  <div :class="status ? 'success' : 'failed'">
    STATUS
  </div>
  <button @click="status = !status">Ubah</button>
  <div :class="[boldClass, greenClass]">TEST</div>
</template>

<script>
export default {
  data() {
    return {
      status: true,
      boldClass: 'bold',
      greenClass: 'success'

    }
  },
}
</script>

<style>
  .success {
    color:teal
  }
  .failed{
    color: cyan
  }
  .bold{
    font-weight: 700;
  }
</style>