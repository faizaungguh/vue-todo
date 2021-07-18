<template>
  <div>
    {{ pesan }}
  </div>
  <span :title='pesan'>bukan teks</span>
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