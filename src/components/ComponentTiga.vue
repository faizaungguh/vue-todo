<template>
<div>Ini Komponen 3</div>
<div>
    {{ providedAuthor }}
  </div>
</template>

<script>
export default {
  inject: ["providedAuthor"],
};
</script>
