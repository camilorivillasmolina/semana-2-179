<template>
    <div>
        <seccion class="mb-5" width="100%">
          <img v-bind:src="member.image" width="100%">
          <h2 class="text-center">
            Team member: {{member.codigo}} {{member.rol}}
          </h2>
          <h2 class="text-center">
            {{member.nombres}}
          </h2>
          <p class="text-justify">
            {{member.descripcion}}
          </p>
        </seccion>
    </div>
</template>

<script>
    export default {
        name: "TeamCard",
        props: ['member']
    }
</script>

<style scoped>

</style>
