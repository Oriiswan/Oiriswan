<template>
   <h1>Counter App</h1>
  <h2 :style="{fontSize: fontSize + 'px'}">{{ counter }}</h2>
  <div>
    <button class="btn-increment" @click="counter++"> Increment
            </button>
            <button class="btn-decrement" @click="counter--"> Decrement</button>
            <button class="btn-increment" @click="fontSize += 5"> Increment font</button>
            <button class="btn-increment" @click = " fontSize -= 5 "> Decrement font</button>
            <button class="btn-change">Change Background Color</button>
           
            <button class="btn-resetcolor">Reset Color</button>
  </div>
            
</template>
<style>
h1 {
   text-align: center;
   font-size: 50px;
   color: white;
}
h2 {
    text-align: center;
    font-size: 50px;
    color: white;
    margin: 0%;
}
body {
    background-color: black 
    
}
div {
    text-align: center;
}
button {
    font-size: 30px;
    box-shadow: 1px 1px 5px rgb(54, 54, 54);
    border: none;
    margin-right: 13px;
    border-radius: 10px;
    cursor: pointer;
}
button:hover {
    background-color: rgb(141, 20, 20);
    transition-duration: 0.4s;
    color: white;
}
</style>
<script setup>
import { ref } from "vue";
const counter = ref(5);
const fontSize = ref(16);
</script>
