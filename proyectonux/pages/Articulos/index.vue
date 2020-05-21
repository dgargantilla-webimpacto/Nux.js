<template>
  <div class="container mt-5">
    <div class="row justify-content-center">
      <div class="col-8">
        <div class="list-group" v-for="(item, index) in articulos" :key="index">
          <nuxt-link :to="`/Articulos/${item.id}`">{{ item.titulo }}</nuxt-link>
        </div>
        <Radio nombre1="Hombre" nombre2="Mujer" />
        <div class="row">
          <div class="col-12">
            <Cumpleaños />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Radio from "@/components/Radio";
import Cumpleaños from "@/components/Cumpleaños";
export default {
  data() {
    return {
      articulos: [
        { id: 1, titulo: "Articulo #1" },
        { id: 2, titulo: "Articulo #2" },
        { id: 3, titulo: "Articulo #3" },
        { id: 4, titulo: "Articulo #4" },
        { id: 5, titulo: "Articulo #5" }
      ]
    };
  },
  components: {
    Radio,
    Cumpleaños
  }
};
</script>
