<script setup>
    import { RouterLink } from 'vue-router';

</script>


<template>
    <header>
        <nav>
            <div class="branding">
                <img src="../assets/logo.svg" alt="image">
                <h1>Vue Todos</h1>
            </div>
            <ul class="nav-routes">
                <RouterLink to="/">Home</RouterLink>
                <RouterLink to="/about">About</RouterLink>
            </ul>
        </nav>
    </header> 
</template>



<style lang="scss" scoped>
    
</style>