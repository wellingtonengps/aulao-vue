<template>
  <div class="componente">
    <h1>Componente Com Dados Reativos Não Primitivos</h1>
    <p>Nome: {{ pessoa.nome }} | Idada: {{ pessoa.idade }}</p>
    <button v-on:click="fazerAniversario()">Fazer Aniversário</button>
    <button @click="mudarNome()">Mudar nome</button>
  </div>
</template>

<!--
<script setup>
import { reactive } from "vue";

const pessoa = reactive({ nome: "Wellingto", idade: 25 });

function fazerAniversario() {
  pessoa.idade += 1;
}

function mudarNome() {
  pessoa.nome = "Ana Maria";
}
</script> -->

<!-- Usando options - API-->

<script>
export default {
  data: function () {
    return {
      pessoa: {
        nome: "Wellington",
        idade: 25,
      },
    };
  },
  methods: {
    fazerAniversario: function () {
      this.pessoa.idade += 1;
    },
    mudarNome: function () {
      this.pessoa.nome = "João";
    },
  },
};
</script>
