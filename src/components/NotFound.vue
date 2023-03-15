<template>
    <div class= "image">
        <img src="@/assets/404-V2.png" alt="">
    </div>
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
    .image{
        display: flex;
        align-items: center;
        flex-wrap: wrap;
        /* width: 350px; */
        justify-content: center;
    }
    ul{
        display: flex;
        justify-content: center;
        align-items: center;
        font-size: 20px;
    }
</style>