<script setup>
import PrimeiroComponente from "@/components/PrimeiroComponente.vue";
import ComDados from "@/components/ComDados.vue";
import ComDadosReativosPrimitivos from "@/components/ComDadosReativosPrimitivos.vue";
import ComDadosReativosNaoPrimitivos from "@/components/ComDadosReativosNaoPrimitivos.vue";
import EscutaEvento from "@/components/EscutaEvento.vue";
import PropriedadesComputadas from "@/components/PropriedadesComputadas.vue";
import PropriedadesAssistidas from "@/components/PropriedadesAssistidas.vue";
</script>

<template>
  <header>Vue</header>
  <PropriedadesAssistidas/>
  <PropriedadesComputadas/>
  <EscutaEvento/>
  <ComDadosReativosNaoPrimitivos />
  <ComDadosReativosPrimitivos />
  <ComDados />
  <PrimeiroComponente />
</template>

<style scoped></style>
