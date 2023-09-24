<template>
    <header class="university-header">
      <div class="university-logo">
        <img src="../assets/Escudo_UNSA.png" alt="Logo de la Universidad" />
      </div>
      <div class="project-info">
        <h1>{{ pName }}</h1>
        <p>{{ cName }}</p>
        <p>{{ sName }}</p>
      </div>
    </header>
  </template>
  
  <script>
  export default {
    name: 'AppHeader',
    data(){
        return{
            pName:'Motor de Búsqueda',
            cName:'Cloud Computing',
            sName:'Barrios Selene - \nFernandez Gino - \nCcari Jose'
        }
    },
    props: {
      projectName: String, // Nombre del proyecto
      courseName: String,  // Nombre del curso
      studentName: String, // Nombre del estudiante
    },
    
  }
  </script>
  
  <style scoped>
  /* Estilos específicos para el encabezado de la universidad */
  .university-header {
    background-color: #007BFF;
    color: white;
    padding: 10px;
    display: flex;
    align-items: center;
  }
  
  .university-logo img {
    width: 100px;
    height: auto;
    margin-right: 20px;
  }
  
  .project-info {
    flex-grow: 1;
  }
  
  .project-info h1 {
    font-size: 24px;
    margin: 0;
  }
  
  .project-info p {
    margin: 5px 0;
  }
  
  </style>
  