<template>
  <!-- mengembalikan nilai string -->
  <div>
    {{ num1 + num2 }}
  </div>
  <!-- dikonversi string to Int -->
  <div>
    {{ parseInt(num1) + parseInt(num2) }}
  </div>
  <!-- menggunakan computed total -->
  <div>
    {{ total }}
  </div>
  <input v-model="num1" />
  <!-- menggunakan computed perbandingan -->
  {{ perbandingan }}
  <input v-model="num2" />
</template>

<script>
export default {
  data() {
    return {
      num1: 0,
      num2: 0,
    };
  },
  computed: {
    total() {
      return parseInt(this.num1) + parseInt(this.num2);
    },
    perbandingan() {
      if (this.num1 > this.num2) {
        return ">";
      }
      return "<";
    },
  },
};
</script>
