<template>
  <div id="app">
    <h1>Todos</h1>
    <Todos v-bind:todos="todos" />
  </div>
</template>

<script>
  import Todos from "@/components/Todos/Todos";

  export default {
  name: 'App',
  components: {
    Todos,
  },
  data(){
    return(
        {
            todos: [
              {
                id: 1,
                title: 'HEllo',
                completed: false,
              },
              {
                id: 4,
                title: 'HEllo',
                completed: false,
              },
              {
                id: 3,
                title: 'HEllo',
                completed: false,
              }
            ]
        }
    )
  }
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
}
h1 {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 20px 0 20px 0 ;
  border-bottom: black 1px solid;
}
  .Todos {
    padding: 10px;
    display: flex;
    flex-direction: column;
    align-items: center;
  }
</style>
