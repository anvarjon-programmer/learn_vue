
<template>
    <div>
      <h1>Counter: {{ counter }}</h1>
      <div class="d-flex gap-2">
        <button @click="onIncrement" class="btn btn-success ">add</button>
        <button @click="onDecrement" class="btn btn-danger">delete</button>
      </div>
    </div>
  </template>
  
  <script>
   export default {
    data(){
      return {
        counter:0
      }
    },
    methods:{
      onIncrement(){
        this.counter += 1
      },
      onDecrement(){
        if(this.counter > 0){
        this.counter -= 1
        }
      },
    }
   }
  </script>
  
  <style></style>
  