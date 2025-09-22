<template>
  <h2>Ciclo de vida</h2>
</template>


<script lang="ts" setup>

import {onMounted, onUnmounted} from "vue"


onMounted(()=> {
    console.log("montado")
})
onUnmounted(()=> {
    console.log("desmontado")
})
</script>
<style></style>
