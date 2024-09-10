<script setup>
import PrimeiroComponente from "@/components/PrimeiroComponente.vue";
import ComDados from "@/components/ComDados.vue";
import ComDadosReativosPrimitivos from "@/components/ComDadosReativosPrimitivos.vue";
import ComDadosReativosNaoPrimitivos from "@/components/ComDadosReativosNaoPrimitivos.vue";
</script>

<template>
  <header>Vue</header>
  <ComDadosReativosNaoPrimitivos />
  <ComDadosReativosPrimitivos />
  <ComDados />
  <PrimeiroComponente />
</template>

<style scoped></style>
