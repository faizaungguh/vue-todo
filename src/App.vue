<template>
<div>Ini Adalah Parent Component</div>
<child-component/>
</template>

<script>
import ChildComponent from './components/ChildComponent.vue'
export default {
  components: { ChildComponent },

}
</script>