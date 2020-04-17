<template>
    <div class="Todos">
        <div v-bind:key="todo.id" v-for="todo in todos">
            <h3 >{{todo.title}}</h3>
        </div>
    </div>
</template>

<script>
    export default {
        name: "Todos",
        props:
            ["todos"]
        ,
    };
</script>

<style>

</style>
