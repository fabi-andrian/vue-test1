<template>
<p :class="{active: count > 5}">Compteur : {{ count }}</p>
<button @click="increment">Incrémenter</button>
<button @click="decrement">Décrémenter</button>
</template>

<script setup>
import {ref} from 'vue'

const count = ref(0)
console.log(count, count.value)
const increment = (event) => {
  console.log(event)
  count.value++
}
const decrement = () => {
  count.value--
}
</script>

<style>
.active {
  color: red;
}
</style>