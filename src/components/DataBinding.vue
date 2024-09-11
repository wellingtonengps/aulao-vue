<template>
  <div class="componente">
    <h1>Compnente com Data Binding</h1>
    <!-- One Way databinding, saindo do javascript e indo para a interface-->
    <!--<input type="text" v-bind:value="valor"></input>-->

    <p>{{ valor }}</p>
    <!--<input type="text" :value="valor" @input="(e) => valor = e.target.value"></input>-->

    <input type="text" v-model="valor"></input>
  </div>
</template>

<script setup>
import { ref } from "vue";
const valor = ref("Vue é muito legal");
</script>
