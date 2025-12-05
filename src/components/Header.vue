<script setup>
import { Icon } from "@iconify/vue";
import logo from "../assets/logo.png";
</script>

<template>
    <header>
        <img :src="logo" alt="">
        <nav>
            <ul>
                <li class="icon">
                    <a class="icon-btn" href="">
                        <Icon class="search-icon" icon="material-symbols:search" />
                    </a>
                </li>
                <li>
                    <a href="">
                        Início
                    </a>
                </li>
                <li>
                    <a href="">
                        Galeria
                    </a>
                </li>
                <li>
                    <a href="">
                        Favoritos
                    </a>
                </li>
                <li class="icon">
                    <a class="icon-btn" href="">
                        <Icon class="user-icon" icon="material-symbols:person" />
                    </a>
                </li>
            </ul>
        </nav>
    </header>
</template>

<style scoped lang="scss">
    header{
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    margin: 3rem;
    font-size: 24px;

    ul{
        display: flex;
        gap: 1.5rem;
        flex-wrap: wrap;
        list-style: none;
        align-items: center;
    }

    .icon, .icon-btn {
        width: 24px;
        height: 24px;
    }

    a {
        text-decoration: none;
        color: black;
    }

    a:hover {
        color: #E1306C;
    }
}
</style>