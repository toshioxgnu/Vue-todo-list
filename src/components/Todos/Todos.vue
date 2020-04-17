<template>
    <div class="Todos">
        <div v-bind:key="todo.id" v-for="todo in todos">
            <TodoItem></TodoItem>
        </div>
    </div>
</template>

<script>
    import TodoItem from "@/components/TodoItem/TodoItem";
    export default {
        components:{
            TodoItem
        },
        props:
            ["todos"]
        ,
    };
</script>

<style>

</style>
