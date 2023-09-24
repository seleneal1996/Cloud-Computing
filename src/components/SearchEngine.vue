<!-- src/components/SearchEngine.vue -->

<template>
    <div class="search-engine">
      <input type="text" class="search-input" placeholder="Buscar en el motor de búsqueda">
      <button class="search-button">Buscar</button>
    </div>
  </template>
  
  <script>
  export default {
    name: 'SearchEngine'
  }
  </script>
  
  <style scoped>
  /* Estilos específicos para el componente de búsqueda */
  .search-engine {
    display: flex;
    align-items: center;
    background-color: #f1f1f1;
    padding: 10px;
    border-radius: 5px;
  }
  
  .search-input {
    flex: 1;
    padding: 5px;
    border: none;
    border-radius: 3px;
  }
  
  .search-button {
    background-color: #007BFF;
    color: white;
    border: none;
    border-radius: 3px;
    padding: 5px 10px;
    margin-left: 10px;
    cursor: pointer;
  }
  </style>
  