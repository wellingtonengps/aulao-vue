<script setup>
  import EmiteEvento from "@/components/EmiteEvento.vue";

  import {ref} from "vue"
  const total = ref(0)

  function atualizarTotal(preco){
      const valor = total.value + preco
      total.value = +valor.toFixed(2)
  }
</script>

<template>
  <div class="componente">
    <h1>Componente que Escuta Evento</h1>
    <p>Total: R${{total}}</p>
    <div class="lista">
      <EmiteEvento item="Item1" :preco="1.99" @teste="atualizarTotal"/>
      <EmiteEvento item="Item2" :preco="34" @teste="atualizarTotal"/>
      <EmiteEvento item="Item3" :preco="10.99" @teste="atualizarTotal"/>
    </div>
  </div>
</template>

<style scoped>
  .lista{
    display: flex;
    justify-content: space-between;
  }
</style>