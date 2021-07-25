<template>
  <div id='lifecycle'>{{ message }}</div>

  <button @click="message = 'tulisan setelah dirender ulang'">Update</button>
</template>

<script>
export default {
  data() {
    return {
      message: 'text awal',
    };
  },
  // dipanggil sebelum created dijalankan
  beforeCreate() {
    console.log('before create');
  },
  // dipanggil sebelum template dirender
  created() {
    console.log('created');
    // console.log(message);
    // console.log(document.getElementById('lifecycle'));
  },
  // dijalankan setelah template dirender
  beforeMount() {
    console.log('before mount');
  },
  // dijalankan setelah template dirender
  mounted() {
    console.log('mounted');
    console.log(message);
    console.log(document.getElementById('lifecycle'));
  },
  // dijalankan ketika ada perubahan atau merender ulang
  beforeUpdate() {
    console.log('before update');
    console.log(document.getElementById('lifecycle').textContent);
  },
  // dijalankan ketika ada perubahan atau merender ulang
  updated() {
    console.log('updated');
    console.log(document.getElementById('lifecycle').textContent);
  },
  // dijalankan kerika component dihancurkan
  beforeUnmount() {
    console.log('before destroy');
  },
  // dijalankan kerika component dihancurkan
  unmounted() {
    console.log('before destroy');
  },
};
</script>
