<template>
  <div>
    {{message}}
  </div>
  <input v-model="message"/>
</template>

<script>
export default {
  data() {
    return {
      message: 'test',
    }
  },
  watch: {
    message(value){
      console.log('perubahan di message itu adalah ' + value);
    }
  }
}
</script>