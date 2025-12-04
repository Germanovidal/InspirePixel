<script setup>
import fotografo from "../assets/banner-img.jpg"
</script>

<template>
    <section class="banner">
        <div>
            <h1>Onde a paisagem vira
                <span>inspiração</span>. </h1>
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

    div { 
        width: 51%;
    }

    h1{
        font-size: 4rem;
        margin-top: 4rem;
        margin-bottom: 1rem;

        span {
            color: #E1306C;
            font-size: 6rem;
        }
    }

    p {
        font-size: 1.4rem;
    }

    img{
        margin-top: 2.5rem;
        width: 40%;
        border-radius: 86px;
    }
</style>