<template>
  <NuxtLink :to="`/products/${card.id}`" class="card">
      <img :src="require(`@/assets/Images/${card.image || 'fe1.jpg'}`)" alt="Fire Extinguisher Image" class="image">
      <h3 class="header">{{card.title}}</h3>
      <p class="snippet">{{card.snippet}}</p>

  </NuxtLink>
</template>

<script>
export default {
  name: 'LargeCard',

  props: ['card'],
}
</script>

<style scoped>
    .card {
        width: 31.5%;
        height: 25rem;
        border: none;
        overflow: hidden;
        padding: 0;
        cursor: pointer;
        color:black;
    }
    .image {
        height: 65%;
        border-radius: 0.5rem;
    }
    .header {
        font-size: 1.15rem;
        margin-top: 0.4rem;
    }

    .card:hover{
        color:black;
        text-decoration: none;
    }

    .snippet {
        color: grey
    }
</style>
