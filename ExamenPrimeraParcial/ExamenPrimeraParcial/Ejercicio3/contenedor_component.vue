<template>
    <div class="contenedor-component">
      <div class="encabezado">
     
        <slot name="encabezado">Encabezado predeterminado</slot>
      </div>
      <div class="contenido">
        
        <slot name="contenido">Contenido predeterminado</slot>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'contenedor-component',
  }
  </script>
  
  <style scoped>
  .contenedor-component {
    border: 1px solid #ccc;
    padding: 10px;
    margin: 10px;
  }
  
  .encabezado {
    background-color: #f0f0f0;
    padding: 5px;
    font-weight: bold;
  }
  
  .contenido {
    padding: 10px;
  }
  </style>
  