<template>
    <seccion class="mb-5" width="100%">
      <img :src="member.foto" width="100%" />
      <h2 class="text-center">{{ member.nombre }}</h2>
      <h3 class="text-center">Código - {{ member.codigo }}</h3>
      <h3 class="text-center">{{ member.rol }}</h3>
      <p class="text-justify">{{ member.descripcion }}</p>
    </seccion>
</template>

<script>
export default {
  name: "TeamCard",
  props: {
    member: Object,
  },
};
</script>

<style scoped>
</style>
