
<template>
    <TodoList location="archive" />
</template>

<script>
import TodoList from '../components/TodoList.vue';

export default { 
    name: "HomePage",
    components: {
        TodoList
    }
}
</script>