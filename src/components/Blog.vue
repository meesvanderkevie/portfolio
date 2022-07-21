<template>
    <h2>Blog</h2>

    <div class="artikel">
        <router-link to="/">
            <h2>Title</h2>
        </router-link>
        <router-link to="/">
            <p>Content</p>
        </router-link>
    </div>
    <div class="artikel">
        <router-link to="/">
            <h2>Title</h2>
        </router-link>
        <router-link to="/">
            <p>Content</p>
        </router-link>
    </div>

    <RouterView/>

</template>
<script>
export default {
    
}
</script>
<style>
    .artikel {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        margin: 1rem;
        padding: 1rem;
        border: 3px solid rgb(0, 0, 0);
        border-radius: 7px;
        background-color: rgb(255, 255, 255);
    }
</style>