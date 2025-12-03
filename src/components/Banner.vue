<script setup>
import fotografo from "../assets/banner-img.jpg"
</script>

<template>
    <section class="banner">
        <div>
            <h1>Onde a paisagem vira
                <span>inspiração</span> </h1>
                <p>Explore paisagens, cores e luzes que inspiram novas histórias através da fotografia.</p>
        </div>
        <img :src="fotografo" alt="">
    </section>
</template>

<style scoped lang="scss">
    .banner{
        display: flex;
        justify-content: space-between;
        margin: 2rem;
    }

    h1{
        font-size: 3rem;
    }
</style>