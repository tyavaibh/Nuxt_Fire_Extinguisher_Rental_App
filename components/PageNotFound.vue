<template>
    <div>
        <h1>Page Not Found!</h1>
        <img :src="require('@/assets/images/fe25.jpg')" alt="Sad Extinguisher Image">
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style scoped>
    div {
        display: flex;
        align-items: center;
        justify-content: center;
        width: 40rem;
        /* border: 2px solid black; */
        margin: auto;
        margin-top: -4.5rem;
    }
    h1 {
        font-size: 5.5rem;
    }
    img {
        width: 12rem;
        margin: 0 auto
    }
</style>