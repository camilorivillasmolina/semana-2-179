<template>
  <div id="app">
      <div id="team" class="container-fluid">
        <div class="row">
          <div class="col" v-for="(item, index) of equipo" :key="index">
            <TeamCard v-bind:member="item"></TeamCard>
          </div>
        </div>
      </div>
  </div>
</template>

<script>
import TeamCard from './components/TeamCard.vue'
export default {
  name: 'App',
  components: {
		TeamCard
  },
  data(){
    return{
      equipo:[
            {
              "codigo": 1,
              "nombres": "Francisco Benitez",
              "descripcion": "Colegio Los Andes, 23 anios de edad, me gusta programar, ver television, jugar futbol y videojuegos, mi comida favorita es la chuleta de cerdo.",
              "rol": "Desarrollador backend",
              "image": "../public/img/fbfoto.png"
            },
            {
              "codigo": 2,
              "nombres": "Alejandro Benavides",
              "descripcion": "Desarrollador Full Stack BackEnd de MisionTIC 2022",
              "rol": "Desarrollador backend",
              "image": "../public/img/pp.jpg"
            },
            {
             "codigo": 3,
              "nombres": "Ana Shirley Montilla",
              "descripcion": "Estudiante de Ingenieria de Sistemas en la UNAD, me gusta el deporte ¡Cualquiera! No había usado Python, Java, ni creado páginas web. Soy de Palmira - Valle del Cauca, pero vivo en Bogotá.",
              "rol": "Desarrollador backend",
              "image": "../public/img/shirley.jpg"
            },
            {
              "codigo": 4,
              "nombres": "Camilo Rivillas",
              "descripcion": "Soy ingeniero de petróleos graduado de la universidad de América, tengo 26 años y me gusta montar montar bicicleta. La ruta que más hago en bicicleta es subir al alto de patios, via a la Calera.",
              "rol": "Desarrollador backend",
              "image": "../public/img/camilo.jpg"
            },
            {
              "codigo": 5,
              "nombres": "Sergio Sandoval",
              "descripcion": "Institución: Misión TIC 2022 - UTP. Edad: La suficiente. Pasatiempos: Algunos mas que otros. Otros: Efectivamente son varios.",
              "rol": "Desarrollador backend",
              "image": "../public/img/PerfilSS.jpg"
            }
      ]  
    }  
  }
}
</script>

