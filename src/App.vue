<template>
<p>Compteur : {{ count }}</p>
<button @click="increment">Incrémenter</button>
<button @click="decrement">Décrémenter</button>
</template>

<script setup>
import {ref} from 'vue'

const count = ref(0)
const increment = () => {
  count.value++
}
const decrement = () => {
  count.value--
}
</script>
