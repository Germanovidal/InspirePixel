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

    <div class="email">
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
        margin: 7rem 3rem 3rem;
        display: flex;
        height: 15rem;
        gap: 25px;

        div {
            width: 24rem;
            line-height: 2rem;
        }

        ul {
            list-style: none;
        }

        ul li a{
            text-decoration: none;
            color: #000000;
        }

        ul li a:hover{
            text-decoration: underline;
        }

        h3 {
            font-size: 24px;
            font-weight: 600;
            margin-bottom: 1rem;
        }
    }

    .redes {
        display: flex;
        justify-content: flex-start;
        align-items: flex-end;
        gap: 10px;

        a img:hover {
            background-color: #E1306C;
            border: solid #E1306C;
            border-radius: 50%;
        }
    }

    .email {
        width: 36.5rem;
    }

    .email-box {
        border: none;
        background-color: #E6E6E63B;
        width: 100%;
        height: 3.125rem;
        padding: 1rem;
        border-radius: 5px;
        font-size: 16px;
    }

    .btn {
        margin-top: 1.25rem;
        font-size: 16px;
        font-weight: bold;
        color: #FFFFFF;
        width: 8.875rem;
        height: 2.5rem;
        border: none;
        background-color: #E1306C;
        border-radius: 5px;
        cursor: pointer;
    }

    .btn:hover{
        background-color: #9d214b;
    }

    @media screen and (max-width: 1440px) {
        footer div {
            width: 18.188rem;
        }
    }

</style>