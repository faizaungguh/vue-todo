<template>
  <div v-if="status">Aku di sini</div>

  <button @click="setStatus">Temukan Aku</button>

  <div v-if="status">true</div>
  <div v-else>false</div>
</template>

<script>
export default {
  data() {
    return {
      status: false
    }
  },
  methods: {
    setStatus(){
      this.status = !this.status
    }
  }
}
</script>