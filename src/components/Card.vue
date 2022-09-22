<template>
  <Grid>
      <slot>Imagen</slot>
      <h2>{{ nombre }}</h2> 
      <h4>{{ descripcion }}</h4><br>
      <h3>{{ costo }}</h3><br>
  </Grid>
</template>

<script>
  import Grid from "./Grid.vue";
  export default{
  props: {
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
      width: 11rem;
      height: 11rem;
      padding: 0.1rem;
      background: rgba(177, 177, 177, 0.297);
  }
 
  
</style>