<template>
  <component-satu />
</template>

<script>
import ComponentSatu from "./components/ComponentSatu.vue";
export default {
  components: { ComponentSatu },
  data() {
    return {
      author: "Ungguh",
    }
  },
  provide(){
    return {
      providedAuthor: this.author,
    }
  }
};
</script>
