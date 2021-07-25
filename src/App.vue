<template>
  <child-component ref="refComponent" @child-click="onPress" />
  <button @click="clickSaya">Button Parent</button>
</template>
<script>
import ChildComponent from "./components/ChildComponent.vue";
export default {
  components: { ChildComponent },
  methods:{
    onPress(val){
      console.log(val)
    },
    clickSaya(){
      this.$refs.refComponent.onClick();
    }
  }
};
</script>
