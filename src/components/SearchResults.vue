<!-- src/components/SearchResults.vue -->

<template>
    <div class="search-results">
      <h2>Resultados de la búsqueda</h2>
      <ul>
        <li v-for="(result, index) in searchResults" :key="index">{{ result }}</li>
      </ul>
    </div>
  </template>
  
  <script>
  export default {
    name: 'SearchResults',
    props: {
      searchResults: Array, // Propiedad para recibir los resultados de búsqueda
    },
  }
  </script>
  
  <style scoped>
  /* Estilos específicos para el componente de resultados */
  .search-results {
    margin-top: 20px;
  }
  </style>
  