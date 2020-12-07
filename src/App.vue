<template>
  <div id="app">
    <section id=" news" class="noticias">
      <div class="container-fluid bg-light">
        <section-api></section-api>
      </div>
    </section>
    <div id="team" class="container-fluid">
      <div class="row justify-content-center mb-5">
        <div class="col mt-5 h-100" v-for="(item, index) of team" :key="index">
          <team-card :member="item"></team-card>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import TeamCard from "./components/TeamCard.vue";
import SectionApi from "./components/SectionApi.vue";

export default {
  name: "App",
  components: {
    TeamCard,
    SectionApi
  },
  data() {
    return {
      team: [
        {
          codigo: 1,
          nombre: "David Felipe Varón Molano",
          descripcion:
            "Estudiante de ingeniería mecánica de la Universidad Nacional de colombia, curioso por la programación, aficionado a los videojuegos y con ganas por mejorar la educación en colombia.",
          rol: "Developement Team",
          imagen: "/assets/davidvaron.jpg",
        },
        {
          codigo: 2,
          nombre: "Julián Andrés López Quintero",
          descripcion: "Director de orquesta y compositor de musica para cine, TV y videojuegos; apasionado por el baile, aficionado a la programacion y a la cocina, dispuesto a aprender algo distinto cada dia y compartir el conocimiento.",
          rol: "Developement Team",
          imagen: "/assets/julianlopez.jpg",
        },
        {
          codigo: 3,
          nombre: "Rubén Darío Candia Parra",
          descripcion: "Ingeniero Industrial y Especialista en gestión de proyectos, apasionado de la lectura, dibujo y el aprendizaje.",
          rol: "Developement Team",
          imagen: "/assets/rubencandia.jpg",
        },
        {
          codigo: 4,
          nombre: "Antonio Morales Correa",
          descripcion: "Tecnólogo en Sistemas de Telecomunicaciones, apasionado de la lectura y videojuegos, en busca de nuevo conocimiento en programación y otras ramas de ella.",
          rol: "Developement Team",
          imagen: "/assets/antoniomorales.jpg",
        },
        {
          codigo: 5,
          nombre: "No Activo",
          descripcion:
            "Estudiante no activo.",
          rol: "Developement Team",
          imagen: "/assets/nn.webp",
        },
      ],
    };
  },
};
</script>

