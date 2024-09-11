<script setup>
  import {defineProps, defineEmits } from "vue"

  const props = defineProps({
    item: String,
    preco: Number
  })

  const emit = defineEmits(
      [
          "teste"
      ])

  function adicionar(){
    emit("teste", props.preco)
  }
</script>

<template>
  <div class="componente">
    <h1>Componete que emite Evento</h1>
    <p>{{item}} (R${{preco.toFixed(2)}})</p>
    <button @click="adicionar">Adicionar ao carrinho</button>
  </div>
</template>

<style scoped>

</style>