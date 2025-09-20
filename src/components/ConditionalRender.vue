<script setup lang="ts">
const num = 7
</script>
<template>

    <div v-if="num < 18">Es menor de edad</div>
    <div v-else>Es mayor de edad</div>
</template>
<style></style>