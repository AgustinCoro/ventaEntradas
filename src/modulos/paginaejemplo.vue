<template>
  <div>
    <h1>Pagina de Ejemplo</h1>
    <v-row>
      <v-col cols="4">
        <v-img
          src="E:\Proyectos\Repositorio Compartido\VUE\ventaEntradas\src\assets\ratablanca-sde.jpg"
          alt="Example image"
          width="400"
          height="300"
          :lazy-src="true"
          aspect-ratio="1.33"
          placeholder="https://example.com/placeholder.jpg"
        />
      </v-col>
      <v-col cols="8"> </v-col>
    </v-row>
  </div>
</template>

<script>
export default {
  name: "EjemploView",
};
</script>

<style></style>
