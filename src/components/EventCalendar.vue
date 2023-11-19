<template>
    
    <div class="event-calendar">
      <div v-for="event in events" :key="event.id" class="event">
        <h3>{{ event.title }}</h3>
        <p>{{ event.date }}</p>
        <p>{{ event.description }}</p>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    props: {
      events: Array
    }
  };
  </script>
  
  <style scoped>

  
  .event-calendar {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
    gap: 20px;
    margin: 30px;
  }
  
  .event {
    border: 1px solid #000000;
    padding: 10px 20px;
    background-color: #FFFF99;
  }
  </style>