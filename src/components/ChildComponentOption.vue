<template>
  <div class="div_child">
    <h2>{{ props.text }}</h2>
    <h2>{{ props.num }}</h2>
  </div>
</template>
<script lang="ts" >
import {defineComponent} from "vue"

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
    setup(props){
      return {props}
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
