<template>
  <div>
    {{ message }}
  </div>

  <child-component
    :model-value="message"
    @update:model-value="message = $event"
  />
</template>

<script>
import ChildComponent from "./components/ChildComponent.vue";

export default {
  components: { ChildComponent },
  data() {
    return {
      message: "",
    };
  },
};
</script>
