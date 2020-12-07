<template>
  <div>
    <div class="row mt-md-5 mt-sm-5 mt-xs-5">
      <!-- cuadro 1 -->
      <div
        class="cuadro 1 col-lg-6 col-xs-12"
        v-for="(movie, index) of movies"
        :key="index"
      >
        <div class="d-flex justify-content-center align-items-center">
          <div class="imagen1 align-self-center mr-3">
            <img
              :src="movie.Poster"
              alt="movie poster"
              width="200"
              height="350"
            />
          </div>

          <div class="noticia-texto">
            <h3 class="noticia-titulo">
              {{ movie.Title }}
            </h3>
            <hr />
            <p class="noticia-parrafo">
              Película del año {{ movie.Year }} que parodia a las clásicas
              películas de terror de los años 80´s y 90's con un humor
              característico de las películas para adolescentes de estados
              Unidos.
            </p>
          </div>
        </div>

        <div class="d-flex container-fluid justify-content-end pb-2 mt-n2">
          <a :href="'https://www.imdb.com/title/' + movie.imdbID" class="btn btn-dark" role="button">Información completa</a
          >
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import axios from "axios";
export default {
  name: "SectionApi",
  data() {
    return {
      movies: null,
    };
  },
  mounted() {
    axios
      .get("http://www.omdbapi.com/?s=scary+movie&type=movie&apikey=b5bcae1a")
      .then((response) => {
        this.movies = response.data.Search.slice(0, 4);
        console.log(this.movies);
      });
  },
};
</script>

<style scoped>
</style>