<template>
<p :style="{color: count > 5 ? 'red' : 'green'}">Compteur : {{ count }}</p>
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
