<script setup>
import { RouterLink } from 'vue-router'
</script>

<template>
    <header>
        <div class="container">
            <RouterLink to="/" class="logo">
                <img src="../assets/logo-white.png" alt="logo-henrique-quintino">
                <h1>Learning Vue</h1>
            </RouterLink>
            <nav>
                <RouterLink to="/" :class="{ 'active-link': $route.path === '/' }">Home</RouterLink>
                <RouterLink to="/about" :class="{ 'active-link': $route.path === '/about' }">About</RouterLink>
            </nav>
        </div>
    </header>
</template>