<!-- Passa componetes de um pai para filho ou ao contrario-->

<template>
  <div class="componente">
    <h1>Componente com Slots</h1>
    <button><slot name="icone" /><slot name="texto"> Botão </slot></button>
  </div>
</template>

<style scoped>
button {
  display: flex;
  align-items: center;
}
</style>
