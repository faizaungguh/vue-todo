<template>
  <teleport to="#target-teleport">
    <home-component />
  </teleport>
</template>

<script>
import HomeComponent from "./components/Home.vue";
export default {
  components: { HomeComponent },
};
</script>
