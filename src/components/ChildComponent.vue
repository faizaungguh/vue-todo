<template>
  <div>
    <span> Ini dari Child </span>
    <button @click="onPress">Child Button</button>
  </div>
</template>

<script>
export default {
  emits: ["child-click"],
  methods: {
    onClick() {
      console.log("click saya");
    },
    onPress() {
      this.$emit("child-click", "value");
    },
  },
};
</script>
