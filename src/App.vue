<template>
<p>Compteur : {{ count }}</p>
<div v-show="count>=5">Bravo vous avez cliqué plus de 5 fois</div>
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
