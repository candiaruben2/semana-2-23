<template>
  <div id="app">
    <section id=" news" class="noticias">
      <div class="container-fluid bg-light">
        <section-api></section-api>
      </div>
    </section>
  </div>
</template>

<script>
import SectionApi from "./components/SectionApi.vue";

export default {
  name: "App",
  components: {
    SectionApi,
  },
};
</script>

