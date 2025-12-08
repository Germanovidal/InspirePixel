<script setup>
import { ref } from "vue"
import { Icon } from "@iconify/vue";
import logo from "../assets/logo.png";
import menuicon from "../assets/icon-menu-mobile.png"

const isMenuOpen = ref(false);

const toggleMenu = () => {
  isMenuOpen.value = !isMenuOpen.value;
};

</script>

<template>
    <header>
        <img :src="logo" alt="logo da Inspire Pixel">
        
        <button class="burger" :class="{ 'active': isMenuOpen }" 
        @click="toggleMenu">
        <img :src="menuicon" alt="">
        </button>

        <nav class="nav-menu" 
            :class="{ 'open': isMenuOpen }">
            <ul>
                <li class="icon">
                    <a class="icon-btn" href="">
                        <Icon class="search-icon mobile" icon="material-symbols:search" />
                    </a>
                </li>
                <li>
                    <a href="" @click="isMenuOpen = false">
                        Início
                    </a>
                </li>
                <li>
                    <a href="" @click="isMenuOpen = false">
                        Galeria
                    </a>
                </li>
                <li>
                    <a href="" @click="isMenuOpen = false">
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
    header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    margin: 3rem;
    font-size: 1.5rem;

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

}

a {
    text-decoration: none;
    color: black;
}

a:hover {
    color: #E1306C;
}

.burger{
    display: none;
    z-index: 20;
}

@media (max-width: 768px) {
    header {
        font-size: 1.875rem;
    }

    .search-icon {
        display: none;
    }

    .burger{
        display: block;
        background-color: #FFFFFF;
        border: none;
    }

    .burger .bar {
        display: block;
        width: 25px;
        height: 3px;
        margin: 5px auto;
        background-color: #333;
        transition: all 0.3s ease-in-out;
    }

    .nav-menu {
        position: fixed;
        top: 0;
        left: 0;
        width: 100%;
        height: 100vh; /* Altura total da tela */
        background-color: white; 
        z-index: 10;
        
        /* Oculta o menu para a esquerda */
        transform: translateY(-100%); 
        transition: transform 0.3s ease-in-out;
    }

    .nav-menu.open {
        transform: translateX(0); 
    }

    .nav-menu ul {
        flex-direction: column;
        align-items: center;
        padding-top: 80px;
    }
}

</style>