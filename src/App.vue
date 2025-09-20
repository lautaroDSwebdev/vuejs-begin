<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import DataComposition from './components/DataComposition.vue';
import ConditionalRender from './components/ConditionalRender.vue';
</script>

<template>
  <!-- <DataComposition /> -->
   <ConditionalRender/>
  <RouterView />
</template>
