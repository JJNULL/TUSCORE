<template>
    <div>
      <h2>Tabla de Partidos</h2>
      <table class="table table-bordered table-striped">
        <thead>
          <tr>
            <th>Fecha</th>
            <th>Equipo Local</th>
            <th>Equipo Visitante</th>
            <th>Resultado</th>
          </tr>
        </thead>
        <tbody>
          <tr v-for="(partido, index) in partidos" :key="index">
            <td>{{ partido.fecha }}</td>
            <td>{{ partido.equipoLocal }}</td>
            <td>{{ partido.equipoVisitante }}</td>
            <td>{{ partido.resultado }}</td>
          </tr>
        </tbody>
      </table>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        partidos: [
          { fecha: '2023-08-01', equipoLocal: 'Equipo A', equipoVisitante: 'Equipo B', resultado: '3 - 2' },
          { fecha: '2023-08-05', equipoLocal: 'Equipo C', equipoVisitante: 'Equipo D', resultado: '1 - 1' },
          { fecha: '2023-08-01', equipoLocal: 'Equipo A', equipoVisitante: 'Equipo B', resultado: '3 - 2' },
          { fecha: '2023-08-01', equipoLocal: 'Equipo A', equipoVisitante: 'Equipo B', resultado: '3 - 2' },
          // Agrega más objetos de partido aquí
        ]
      };
    }
  };
  </script>
  
  <style scoped>
  /* Puedes agregar estilos específicos si es necesario */
  </style>
  