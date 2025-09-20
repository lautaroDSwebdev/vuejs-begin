<script lang="ts">
import { defineComponent, ref } from 'vue'

export default defineComponent({
  name: 'FirstCounterComposition',
  setup() {
    const counter = ref(0)
    const counterNumberInc = () => {
      counter.value++
      console.log(counter)
    }
    const counterNumberDec = () => {
      counter.value--
      console.log(counter)
    }
    const reset = () => {
      counter.value = 0
    }
    return { counter, 
        counterNumberDec,
         counterNumberInc ,
         reset
        }
  },
})
</script>

<template>
  <div>
    <button @click="counterNumberDec">boton decremental</button>
    <button @click="counterNumberInc">boton incremental</button>
    <button @click="reset">boton reset</button>
  </div>
  <div>data: {{ counter }}</div>
</template>

<style></style>
