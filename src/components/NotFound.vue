<template>
    <h2>404-Page not found</h2>
    <ul>
        <router-link to="/">Go to main page</router-link>
    </ul>
</template>

<script>
export default{
    name: 'NotFound'
}
</script>

<style scoped>
    h2{
        padding-top: 5%;
        text-align: center;
        font-size: 30px;
    }
    ul{
        display: flex;
        justify-content: center;
        align-items: center;
    }
</style>