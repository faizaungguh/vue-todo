<template>
  <div v-once>{{ message }}</div>
  <button @click="message = 'berubah loh'">Update</button>
</template>

<script>
export default {
  data() {
    return {
      message: 'Hi bro'
    };
  },
};
</script>
