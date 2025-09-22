<template>
    <p v-bind:class="{'succes': info}">informacion</p>
</template>

<script setup lang="ts">
    const info = true
    // const fail = true
</script>
<style>
.succes{
    color: chartreuse;
}
.fail{
    color: red;
}
</style>