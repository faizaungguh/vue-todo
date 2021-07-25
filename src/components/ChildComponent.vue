<template>
  <input
    :value="modelValue"
    @input="$emit('update:model-value', $event.target.value)"
  />
</template>

<script>
export default {
  props: ["modelValue"],
};
</script>
