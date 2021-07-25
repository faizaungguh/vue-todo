<template>
  <div>
    {{ message }}
  </div>
  <hr />
  <!-- <child-component
    :model-value="message"
    @update:model-value="message = $event"
  /> -->
  
  <!-- v-model merupakan sintatic sugar dari metode di atas -->
  <child-component v-model="message"/>
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
