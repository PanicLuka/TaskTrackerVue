<template>
    <header>
        <h1>{{ title }}</h1>
        <Button @add-task="$emit('add-task')" :title="isShown ? 'Close' : 'Add Task'" 
        :color="isShown ? 'red' : 'green'"/>
    </header>
    
</template>


<script>
import Button from './Button.vue'

export default {
    name: 'Header',
    components: {
        Button,
        
    },
    props: {
        title: String,
        isShown: Boolean
    },
    // emits: ['add-task']
    
}
</script>

<style scoped>
header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 20px;
}
</style>