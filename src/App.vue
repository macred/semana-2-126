<template>
  <div id="app">
    <div class="container-fluid">
      
          <section-api></section-api>
        </div>

        <div class="container-fluid">
          <div class="row justify-content-center mb-5">
            <div class="col mt-5" v-for="(item, index) of team" :key="index">
              <team-card v-bind:member="item"></team-card>
            </div>
          </div>
        </div>
      </div>
    
</template>

<script>
import TeamCard from "./components/TeamCard.vue";
import SectionApi from "./components/SectionApi.vue";

export default {
  components: { TeamCard,
  SectionApi },
  name: "App",
  data() {
    return {
      team:[
        {
          codigo: 1,
          nombre :'Andres F. Giraldo',
            rol : 'Scrum Master',
            info : 'Vivo en la cuidad de Cali. Apasionado de la electrónica y el desarrollo de software. Mis pasatiempos son la lectura, videojuegos y Anime',
            img :'https://image.freepik.com/vector-gratis/programador-hombre-trabajando-codigo-computadora-portatil-programador-codificacion_88272-1380.jpg',

        },
        {
          codigo: 2,
          nombre :'Malory Camargo',
            rol : 'Backend',
            info : 'Vivo en la ciudad de Bogotá, me interesa el desarrollo tecnológico aplicado a las humanidades digitales. Mis pasatiempos son la músicay los emprendimientos culturales.',

            img :'https://image.freepik.com/vector-gratis/ilustracion-colorida-programador-femenino-trabajando_23-2148277397.jpg',

        },
        {
          codigo: 3,
          nombre :'Yody Tovar',
            rol : 'Frontend',
            info : 'Vivo en Fusagasugá, me dedico al comercio electrónico y me apasiona todo lo que se relacione con marketing digital, mis pasatiempos son la lectura y el deporte.',
            img :'https://static.vecteezy.com/system/resources/previews/000/227/854/non_2x/female-developer-vector.jpg',

        }
      ],
      SectionApi
    };
  },
};
</script>

