<template>
  <div>
    {{ pesan }}
  </div>
  <span :title='message'>bukan teks</span>
</template>

<script>
export default {
  data() {
    return {
       pesan : 'Sugeng Siang'
    }
  },
}
</script>