
<template>
    <h1>To do list</h1>
    <VueDepthCard>
    </VueDepthCard>
    <TodoList location="home" />
</template>

<script>
import TodoList from '../components/TodoList.vue';
import VueDepthCard from 'vue-depth-card'

export default { 
    name: "HomePage",
    components: {
        TodoList,
        VueDepthCard
    }
}
</script>
