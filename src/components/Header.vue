<template>

    <RouterLink to="/">Home</RouterLink>
    <RouterLink to="/">O&O</RouterLink>
    <RouterLink to="/">Projecten</RouterLink>
    
</template>

<style>
    .nav {
        display: flex; 
        justify-content: center;
        align-items: center;
        background-color: #f5f5f5;
        gap: 1rem;
        border-width: 1px solid black;
        border-radius: 1.5rem;
    }

    .nav a {
        text-decoration: none;
        color: black;
        font-weight: bold;
        font-size: 1.5rem;
        font-family: 'Open Sans', sans-serif;
        transition: all 0.4s ease-in-out;
    }

    .nav a:hover {
        color: #6b6b6b;
        font-size: 2rem;
        background-color: lightgray;
        border-radius: 1rem;
    }
</style>