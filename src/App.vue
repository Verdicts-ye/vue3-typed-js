<template>
  <vuetyped :string="['你好！']">
    <div class="typing"></div>
  </vuetyped>
</template>

<script setup>
import vuetyped from "vue3typed/libs/typed";
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
