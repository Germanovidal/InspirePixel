<script setup>
    import face from "../assets/facebook.png";
    import instagram from "../assets/instagram.png";
    import linkedin from "../assets/linkedin.png";
    import twitter from "../assets/twitter.png";
</script>

<template>
<footer>
    <div>
        <h3>Contato</h3>
        <ul>
            <li>
                <a href="">contato@inspiralens.com</a>
            </li>
            <li>
                <a href="">Central de ajuda</a>
            </li>
            <li>
                <p>Rio de Janeiro - Brasil</p>
            </li>
        </ul>
    </div>

    <div>
        <h3>Sobre</h3>
        <ul>
            <li>
                <a href="">Politicas</a>
            </li>        
            <li>
                <a href="">Politicas de privacidade</a>
            </li>
            <li>
                <a href="">Blog</a>
            </li>
        </ul>
    </div>

    <div class="redes">
        <a href=""><img :src=face alt=""></a>
        <a href=""><img :src=linkedin alt=""></a>
        <a href=""><img :src=instagram alt=""></a>
        <a href=""><img :src=twitter alt=""></a>
    </div>

    <div>
        <h3>Assine nossa newsletter</h3>
        <ul>
            <li>
                <input class="email-box" type="email" name="" id="" placeholder="Seu email">
            </li>
            <li>
                <button class="btn">Inscreva-se</button>
            </li>
        </ul>
    </div>    
</footer>
</template>

<style scoped lang="scss">
    footer {
        margin: 2rem;
        display: flex;
        justify-content: space-between;
        height: 15rem;

        ul {
            list-style: none;
        }

        ul li a{
            text-decoration: none;
            color: #000000;
        }
    }

    .email-box {
        border: none;
        background-color: #E6E6E63B;
        width: 100%;
        height: 2rem;
        padding: 1rem;
        border-radius: 5px;
    }

    .btn {
        color: #FFFFFF;
        width: 8.5rem;
        height: 2rem;
        border: none;
        background-color: #E1306C;
        border-radius: 5px;
        cursor: pointer;
    }

    .btn:hover{
            background-color: #9d214b;
        }

</style>