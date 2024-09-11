<script setup>
import PrimeiroComponente from "@/components/PrimeiroComponente.vue";
import ComDados from "@/components/ComDados.vue";
import ComDadosReativosPrimitivos from "@/components/ComDadosReativosPrimitivos.vue";
import ComDadosReativosNaoPrimitivos from "@/components/ComDadosReativosNaoPrimitivos.vue";
import DataBinding from "@/components/DataBinding.vue";
import ComProps from "./components/ComProps.vue";
</script>

<template>
  <header>Vue</header>
  <ComProps item="Lápis" :preco="2.5" />
  <DataBinding />
  <ComDadosReativosNaoPrimitivos />
  <ComDadosReativosPrimitivos />
  <ComDados />
  <PrimeiroComponente />
</template>

<style scoped></style>
