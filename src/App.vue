<template>
  <div id="app">
    <CabeceraPrincipal></CabeceraPrincipal>
    <SeccionServicios></SeccionServicios>
    <SeccionNoticias></SeccionNoticias>
    <div id="team" class="container-fluid">
    <div class="row">
    <div class="col" v-for="(integrante, index) of equipo" :key="index">
    <TeamCard :member="integrante"></TeamCard>
    </div>
    </div>
    </div>
    <SeccionFooter></SeccionFooter>
  </div>
</template>

<script>
import CabeceraPrincipal from "./components/CabeceraPrincipal.vue"
import SeccionServicios from "./components/SeccionServicios.vue"
import SeccionNoticias from "./components/SeccionNoticias.vue"
import SeccionFooter from "./components/SeccionFooter.vue"
import TeamCard from "./components/TeamCard.vue"
import IntegrantesEquipo from "../public/equipo.json"

export default {
  name: 'App',
  components: {
    CabeceraPrincipal,
    SeccionServicios,
    SeccionNoticias,
    SeccionFooter,
    TeamCard
  },
  data() {
    return {
      equipo: IntegrantesEquipo.equipo
    }
  }
}
</script>

