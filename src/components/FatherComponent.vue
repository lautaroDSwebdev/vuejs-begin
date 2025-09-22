<template>
  <div class="styled_div">
    <ChildCponent v-for='data in lista' :key='data.num' :text='data.text' :num='data.num' />
  </div>
</template>
<script lang="ts" setup>
import ChildCponent from '@/components/ChildComponent.vue'


interface Data {
  text: string
  num: Number
}

const lista: Data[] = [
  {
    text: 'post 1',
    num: 54645,
  },
  {
    text: 'post 2',
    num: 56576,
  },
  {
    text: 'post 3',
    num: 7655,
  },
  {
    text: 'post 4',
    num: 7655,
  },
]
</script>
<style scoped>
.styled_div {
  display: flex;
  flex-flow: wrap;
  justify-content: space-around;
  gap: 5px;
}
</style>
