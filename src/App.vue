<template>
  <child-component>
    <template v-slot:default>
      Ini default slot
    </template>
    <template v-slot:slot2>
      Ini slot2
    </template>
    <template v-slot:slot3>
      Ini slot3
    </template>
  </child-component>
</template>

<script>
import ChildComponent from "./components/ChildComponent.vue";

export default {
  components: { ChildComponent },
};
</script>
