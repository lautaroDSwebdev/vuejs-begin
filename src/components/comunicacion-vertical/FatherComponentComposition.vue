<template>
  <div class="styled_div">
    
    <ChildComponentOption 
    v-for='data in lista'
     :key='data.num'
    :text='data.text'
     :num='data.num'
      @Saludar="Mensaje"


      />
  </div>
</template>



<script lang="ts" setup>
import { lista } from '@/mock/mock';
import ChildComponentOption from './ChildComponentOption.vue';


// Funcion padre
const Mensaje = (params: string) => {
    alert(params)
    console.log("Esto es desde el padre")
}


</script>
<style scoped>


.styled_div {
  display: flex;
  flex-flow: wrap;
  justify-content: space-around;
  gap: 5px;
}
</style>
