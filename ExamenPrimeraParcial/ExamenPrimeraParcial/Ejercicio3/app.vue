<template>
  <div>
    <contenedor-component>
      <template #encabezado>
        <h1>Este es el encabezado personalizado</h1>
      </template>
      
      <template #contenido>
        <p>Este es el contenido personalizado.</p>
      </template>
    </contenedor-component>
  </div>
</template>

<script>
import ContenedorComponent from './contenedor_component.vue';

export default {
  components: {
    ContenedorComponent,
  },
}
</script>
