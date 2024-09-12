<script setup>
import PrimeiroComponente from "@/components/PrimeiroComponente.vue";
import ComDados from "@/components/ComDados.vue";
import ComDadosReativosPrimitivos from "@/components/ComDadosReativosPrimitivos.vue";
import ComDadosReativosNaoPrimitivos from "@/components/ComDadosReativosNaoPrimitivos.vue";
import DataBinding from "@/components/DataBinding.vue";
import ComProps from "./components/ComProps.vue";
import EscutaEvento from "@/components/EscutaEvento.vue";
import PropriedadesComputadas from "@/components/PropriedadesComputadas.vue";
import PropriedadesAssistidas from "@/components/PropriedadesAssistidas.vue";
import RenderizacaoCondicional from "./components/RenderizacaoCondicional.vue";
import RenderizacaoListas from "./components/RenderizacaoListas.vue";
import Slots from "./components/Slots.vue";

const cachorrosDoJoao = [
  { nome: "Totó", idade: 2 },
  { nome: "Laika", idade: 8 },
  { nome: "Flor", idade: 4 },
];
</script>

<template>
  <header>Vue</header>
  <Slots>
    <template v-slot:icone>
      <svg
        xmlns="http://www.w3.org/2000/svg"
        width="24"
        height="24"
        viewBox="0 0 24 24"
        fill="none"
        stroke="currentColor"
        stroke-width="2"
        stroke-linecap="round"
        stroke-linejoin="round"
        class="icon icon-tabler icons-tabler-outline icon-tabler-activity-heartbeat"
      >
        <path stroke="none" d="M0 0h24v24H0z" fill="none" />
        <path d="M3 12h4.5l1.5 -6l4 12l2 -9l1.5 3h4.5" />
      </svg>
    </template>
    <template v-slot:texto> Sinal Vital </template>
  </Slots>
  <RenderizacaoListas nome="Maria" :cachorros="[]" />
  <RenderizacaoListas nome="João" :cachorros="cachorrosDoJoao" />
  <RenderizacaoCondicional nome="Maria" :qntd-cachorros="2" />
  <PropriedadesAssistidas />
  <PropriedadesComputadas />
  <ComProps item="Lápis" :preco="2.5" />
  <DataBinding />
  <EscutaEvento />
  <ComDadosReativosNaoPrimitivos />
  <ComDadosReativosPrimitivos />
  <ComDados />
  <PrimeiroComponente />
</template>

<style scoped></style>
