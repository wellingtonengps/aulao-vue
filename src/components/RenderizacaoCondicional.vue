<script setup>
import { defineProps } from "vue";

defineProps({
  nome: String,
  qntdCachorros: Number,
});
</script>

<template>
  <div class="componente">
    <h1>Componetne com Renderização Condicional</h1>
    <p>Nome: {{ nome }}</p>
    <p v-if="qntdCachorros === 0">Não tem Cachorro</p>
    <p v-else-if="qntdCachorros === 1">Tem um Cachorro</p>
    <p v-else>Tem muitos Cachorros</p>
  </div>
</template>

<style scoped></style>
