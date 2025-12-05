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
        width: 18.188rem;
        height: 31.25rem;
        
        img {
            width: 100%;
            height: 100%;
            border-radius: 10px;
        }
    }
</style>