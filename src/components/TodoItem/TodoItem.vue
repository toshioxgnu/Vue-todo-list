<template>
    <div class="TodoItem">
        <h3>{{todo.title}}</h3>
        <input type="checkbox" value=" {{todo.completed}} ">
    </div>
</template>

<script>
    export default {
        props: {

        },
    };
</script>

<style>

</style>