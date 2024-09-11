<script setup>
import PrimeiroComponente from "@/components/PrimeiroComponente.vue";
import ComDados from "@/components/ComDados.vue";
import ComDadosReativosPrimitivos from "@/components/ComDadosReativosPrimitivos.vue";
import ComDadosReativosNaoPrimitivos from "@/components/ComDadosReativosNaoPrimitivos.vue";
<<<<<<< HEAD
import DataBinding from "@/components/DataBinding.vue";
import ComProps from "./components/ComProps.vue";
=======
import EscutaEvento from "@/components/EscutaEvento.vue";
import PropriedadesComputadas from "@/components/PropriedadesComputadas.vue";
import PropriedadesAssistidas from "@/components/PropriedadesAssistidas.vue";
>>>>>>> 7c40d238ab35b30dc24922acd671f8496d33d56b
</script>

<template>
  <header>Vue</header>
<<<<<<< HEAD
  <ComProps item="Lápis" :preco="2.5" />
  <DataBinding />
=======
  <PropriedadesAssistidas/>
  <PropriedadesComputadas/>
  <EscutaEvento/>
>>>>>>> 7c40d238ab35b30dc24922acd671f8496d33d56b
  <ComDadosReativosNaoPrimitivos />
  <ComDadosReativosPrimitivos />
  <ComDados />
  <PrimeiroComponente />
</template>

<style scoped></style>
