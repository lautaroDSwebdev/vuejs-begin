<script setup lang="ts">
import { ref, type Ref } from 'vue'

type Lista ={
    data: string
}

const lista: Ref<Lista[]> = ref([
  {
    data: 'hola1',
  },
  {
    data: 'hola2',
  },
  {
    data: 'hola3',
  },
])
</script>

<template>
  <div>
    <p v-for="e in lista" v-bind:key="e.data">{{ e.data }}</p>
  </div>
</template>
