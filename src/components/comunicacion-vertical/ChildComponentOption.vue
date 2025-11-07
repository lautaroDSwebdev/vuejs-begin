<template>
  <div class="div_child">
    <h2>{{ props.text }}</h2>
    <h2>{{ props.num }}</h2>
    <button @click="algo">Decir hola</button>
    <!-- <input type="text" v-model="something"> -->
  </div>
</template>
<script lang="ts" >
import {defineComponent, ref, type Ref} from "vue"

export default defineComponent({
  name: "ChildComponentOption",
  props: {
      text:{
        type: String,
        required: true
      },
      num:{
        type: Number,
        required: true
      }
    },
    // Comunicacion ascendente con el emit
    emits: ["Saludar"],
    setup(props, {emit}){

      
      const algo = () => {
        emit("Saludar", "Hola que onda")
      }
      const something:Ref<string> = ref("")
      
      return {props, algo, something}
    }
})
</script>

<style scoped>
.div_child{
    background: #826db3;
    padding: 10px;
    border-radius: 5px;
}
</style>
