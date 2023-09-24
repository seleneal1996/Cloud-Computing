<!-- src/components/Footer.vue -->
<template>
    <footer class="app-footer">
      <div class="footer-content">
        <div>UNSA</div>
        <div>{{ year }}-B</div>
      </div>
    </footer>
  </template>
  
  <script>
  export default {
    name: 'AppFooter',
    data() {
      return {
        year: 2023,
      };
    },
  }
  </script>
  
  <style scoped>
  /* Estilos específicos para el componente de pie de página */
  .app-footer {
    background-color: #f1f1f1;
    text-align: center;
    padding: 10px;
    position: absolute;
    bottom: 0;
    width: 100%;
  }
  
  .footer-content {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
  }
  
  .footer-content div {
    margin: 5px;
  }
  </style>
  