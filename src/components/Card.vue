<script setup>
    defineProps(["imagem"]);
</script>

<template>
    <div class="card">
        <img :src="imagem" alt="Imagens do card">
    </div>
</template>

<style scoped lang="scss">
    .card {
        width: 26rem;
        height: 40rem;
        
        img {
            width: 100%;
            height: 100%;
            border-radius: 10px;
            object-fit: cover;
        }
    }

    @media screen and (max-width: 1440px) {
        .card {
            width: 18.188rem;
            height: 31.25rem;
        }
    }
</style>