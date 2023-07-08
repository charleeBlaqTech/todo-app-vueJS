<script setup>
import { ref , reactive} from 'vue';
    const todo = ref("");
    const todos=[]
    const createTodoFunc=()=>{
        return(todos.push(todo));
    }
    
    //const todoState = reactive("");
</script>

<template>
    <div class="input-wrapper">
        <input type="text" name="" id="" v-model="todo">
        <button @click="createTodoFunc">Create</button>
    </div>
    <p>{{ todo }}</p>
    <div v-for="item in todos" :key="item">
        <p>{{ item }}</p>
    </div>
    
</template>



<style lang="scss" scoped>
    .input-wrapper {
        display: flex;
        transition: 250ms ease;
        border: 2px solid #41b080;
        input{
            width: 100%;
            padding: 8px 6px;

        }
        button{
            padding: 8px 16px;
            cursor: pointer;
        }
    }
</style>