<template>
  <div class="componente">
    <h1>Componente Com Dados Reativos</h1>
    <p>Nome: {{ nome }} | Idada: {{ idade }}</p>
  </div>
</template>

<script setup>
const nome = "Wellington";
const idade = 25;
</script>
