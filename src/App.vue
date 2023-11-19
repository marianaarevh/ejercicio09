<template>
  <h1>Calendario de Eventos</h1>
  <EventCalendar :events="eventList" />
</template>

<script>
import EventCalendar from '@/components/EventCalendar.vue';

export default {
  name: 'App',
  components: {
    EventCalendar
  },
  data() {
    return {
      eventList: [
      {
          id: 1,
          title: "Reunión de equipo",
          date: "2023-11-20",
          description: "Discutir los progresos del proyecto y asignar tareas para la próxima semana."
        },
        {
          id: 2,
          title: "Conferencia de Desarrolladores",
          date: "2023-11-25",
          description: "Asistir a la conferencia anual de desarrolladores para aprender sobre las últimas tecnologías."
        },
        {
          id: 3,
          title: "Entrenamiento de Vue.js",
          date: "2023-12-02",
          description: "Participar en un curso de capacitación intensivo sobre Vue.js para mejorar habilidades de desarrollo."
        },
        {
          id: 4,
          title: "Lanzamiento de Producto",
          date: "2023-12-10",
          description: "Presentación del nuevo producto a clientes y socios importantes."
        }
      ]
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: black;
  margin-top: 60px;
}

body{
  background-image: url("./assets/bg.jpg");
}

h1{
    font-size: 2.2rem;
    font-weight: 800;
    color: black;
    -webkit-text-stroke-width: 1px; 
    -webkit-text-stroke-color: #ffffffcf; 
  }
</style>
