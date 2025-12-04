<script setup>
import Card from './Card.vue';
</script>

<template>
    <h2>Inspire-se</h2>
    <section class="inspire">
    <Card
      imagem="https://i.pinimg.com/736x/1b/d1/e4/1bd1e490c549621df6c2aa68fc28fe99.jpg"
    />
    <Card
      imagem="https://i.pinimg.com/1200x/98/66/cf/9866cf7b3f353137190b0e5d7b275e7b.jpg"
    />
    <Card
      imagem="https://i.pinimg.com/1200x/5d/6b/e2/5d6be230b3a36c866fc8abe63b87dcf1.jpg"
    />
  </section>
</template>

<style scoped lang="scss">
    .inspire, h2{
        display: flex;
        justify-content: space-between;
        font-size: 2.5rem;
        font-weight: normal;
        gap: 10px;
        margin: 2rem;
    }
</style>