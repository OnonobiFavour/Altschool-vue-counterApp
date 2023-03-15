<template>
    <section>

        <div class= "image">
            <img src="@/assets/404-V2.png" alt="">
        </div>
        <ul>
            <router-link to="/">Go to main page</router-link>
        </ul>
    </section>
</template>

<script>
export default{
    name: 'NotFound'
}
</script>

<style scoped>
    section{
        display: flex;
        align-items: center;
        flex-wrap: wrap;
        justify-content: center;
    }
    .image{
        width: 300px;
        height: 300px;
    }
    ul{
        display: flex;
        justify-content: center;
        align-items: center;
        font-size: 20px;
    }
</style>