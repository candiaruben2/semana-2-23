<template>
  <div>
      <div class="card bg-dark text-white">
        <img class="card-img-top" style="height: 200px; object-fit: cover; width: 100%" :src="member.imagen" alt="Card image cap">
        <div class="card-body">
          <h6 class="card-title text-center">{{ member.nombre }}</h6>
          <p class="card-text" style="font-size: 12px">{{ member.descripcion }}</p>
        </div>
        <div class="card-footer">
          <small class="text-light">{{ member.rol }}</small> <br>
          <small class="text-light">Código {{ member.codigo }}</small>
        </div>
      </div>
    </div>
</template>

<script>
export default {
  name: "TeamCard",
  props: ["member"],
};
</script>

<style scoped>
</style>
