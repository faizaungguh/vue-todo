<template>
  <div>Ini Adalah Parent Component</div>
  <child-component text="test aja" />
  <child-component :text="message"/>
</template>

<script>
import ChildComponent from "./components/ChildComponent.vue";
export default {
  components: { ChildComponent },
  data() {
    return {
      message: 'Haiii'
    }
  },
};
</script>
