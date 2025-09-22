<template>
  <div class="div_child">
    <h2>{{ props.text }}</h2>
    <h2>{{ props.num }}</h2>
  </div>
</template>
<script lang="ts" setup>

interface Data {
  text: string
  num: number
}

const props = defineProps<Data>()

</script>
<style scoped>
.div_child{
    background: #826db3;
    padding: 10px;
    border-radius: 5px;
}
</style>
