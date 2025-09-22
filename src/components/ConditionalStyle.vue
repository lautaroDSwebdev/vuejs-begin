<template>
  <p v-bind:style="{color: color_change}">informacion</p>
  <button @click="handleClick">cambiar color</button>
</template>

<script setup lang="ts">
import { ref } from 'vue'

const color_change = ref('#0f82e0')
const handleClick = () => {color_change.value = "#000"}
</script>


<style>

</style>
