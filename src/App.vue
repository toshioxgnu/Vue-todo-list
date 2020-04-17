<template>
  <div id="app">
    <h1>Todos</h1>
    <Todos v-bind:todos="todos" />
  </div>
</template>

<script>
  import Todos from "./components/Todos/Todos";
  import TodoItem from "@/components/TodoItem/TodoItem";
  export default {
  name: 'App',
  components: {
    Todos,
    TodoItem,
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
</style>
