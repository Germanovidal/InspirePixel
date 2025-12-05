<script setup>
import Card from './Card.vue';
// importando o axios -> é uma biblioteca JS para fazer requisições HTTP
import axios from "axios";
// importamos o ref -> uma funcionalidade que permite criar variaveis reativas 
import { ref } from 'vue';

// criar uma variável reativa que vai receber a lista de imagens da api
const imagens = ref([]);

// função assincrona ->
 async function carregarImagens() {
  // res -> resposta da API  
  // AXIOS pegar os dados GET axios.get()
  // await == espera fi tão buscando as imagens
  const res = await axios.get("https://picsum.photos/v2/list?page=5&limit=12");

  imagens.value = res.data;

  console.log(res)
}

carregarImagens()

</script>

<template>
    <h2>Inspire-se</h2>
    <section class="inspire">
    <Card
      v-for="img in imagens"
      :imagem="img.download_url"
    />
  </section>
</template>

<style scoped lang="scss">
  .inspire, h2{
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    font-size: 2.5rem;
    font-weight: normal;
    gap: 25px;
    margin: 3rem;
    
  }
</style>