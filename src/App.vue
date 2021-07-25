<template>
  <child-component>
    <template v-slot:default="props">
      <span>Judul : {{ props.data }}</span>
    </template>
    <template v-slot:slot2="{content}">
      <span>Judul : {{ content }}</span>
    </template>
    <template v-slot:slot3="{data}">
      <span>Judul : {{ data }}</span>
    </template>
  </child-component>
</template>

<script>
import ChildComponent from "./components/ChildComponent.vue";

export default {
  components: { ChildComponent },
};
</script>
