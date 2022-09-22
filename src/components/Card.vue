<template>
  <Grid>
      <img :src="url" :alt="nombre">
      <h2>{{ nombre }}</h2> 
      <h4>{{ descripcion }}</h4><br>
      <h3>{{ costo }}</h3><br>
      <a :href="url" target="_blank">Comprar</a>
  </Grid>
</template>

<script>
  import Grid from "./Grid.vue";
  export default{
  props: {
      url: {
          String,
      },
      nombre: {
          String,
      },
      descripcion: {
          String,
      },
      costo: {
          String,
      },
  },
  components: { Grid },
};
</script>

<style scopet>

  img{
      width: 8  rem;
      height: 8rem;
      padding: 0.5rem;
      background: snow;
      border-radius: 30px;
  }
  a{
      text-decoration: none;
      color: rgb(255, 255, 255);
      background: #ffe4c0cc;
      padding: 0.3rem;
      border-radius: 5px;
      border: 1px solid #ffffff;
      margin-bottom: 60px;
  }
  
</style>